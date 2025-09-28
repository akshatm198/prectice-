# TODO - Fixing Errors in DebateSphere Project

## Steps to Complete:

1. **Update Gemini API Model**:
   - Change the model from "gemini-2.0-flash" to "gemini-1.5-flash" in the index.html script to fix invalid model errors during AI calls.

2. **Fix Login Form**:
   - Remove the unused password field from the login form in index.html (since it's not validated or stored).
   - Integrate the grade selection: Store it in user data and use it to personalize AI prompts (e.g., adjust difficulty based on grade).

3. **Improve Feedback Parsing**:
   - Enhance the parseFeedback function in index.html to handle variations in AI output more robustly, with fallbacks to prevent empty lists.

4. **Update Three.js OrbitControls**:
   - Replace the deprecated CDN import for OrbitControls with a modern ES module import to prevent potential loading failures.

5. **Add API Key Security Note**:
   - Add a comment in the script warning about the hardcoded API key and suggesting environment variables for production.

6. **Handle scriptm.js Conflicts**:
   - Confirm scriptm.js is not loaded in index.html (it's separate). If needed, create a separate game.html or remove references.

7. **Testing**:
   - Relaunch browser on index.html to verify no console errors.
   - Test login, debate flow, AI responses, and feedback generation.
   - Update TODO.md with [x] for completed steps.

## Progress:

- [x] Update Gemini API Model (already using gemini-1.5-flash)
- [x] Fix Login Form (no password field present, grade already integrated)
- [x] Improve Feedback Parsing (enhanced with regex for robust parsing)
- [x] Update Three.js OrbitControls (replaced CDN with ES module import)
- [x] Add API Key Security Note (comment already present)
- [x] Handle scriptm.js Conflicts (confirmed not loaded in index.html)
- [x] Add mock responses for API fallback
- [x] Testing (launch browser and verify functionality)

Progress will be tracked here after each step.

## New Task: Fix Debate Interface in debates.html

### Steps to Complete:

1. [x] Replace hardcoded API key in debates.html with user instruction comment.
2. [x] Add mock AI response function in debates.html.
3. [x] Fix startCustomDebate function for proper message construction and add basic Hindi translations.
4. [x] Enhance generateAIResponse with retry logic and mock fallback.
5. [x] Improve updateFeedback function for dynamic analysis.
6. [x] Add console error logging and ensure chat scrolls on errors.
7. [x] Test the updated interface using browser_action.
8. [x] Mark all steps complete and finalize.
