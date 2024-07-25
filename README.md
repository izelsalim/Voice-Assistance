# Step-by-Step Guide to Building Your Own Voice Assistant in python

<div>
  <img src="https://github.com/salimizel/Voice-Assistance/blob/master/gif.gif" style="width: 20%;">
</div>

## Voice Assistant Script Overview

### Key Features

1. **Speech Recognition and Text-to-Speech:**
   - Utilizes `speech_recognition` for converting speech to text (`listen()` function).
   - Employs `pyttsx3` for converting text to speech (`speak()` function).
   - Allows adjustment of speech rate and voice selection (`engine.setProperty()`).

2. **Command Handling:**
   - Implements a command cache (`command_cache`) to store and retrieve recognized commands and their results, enhancing efficiency.
   - Supports commands such as opening and closing applications (`open chrome`, `close chrome`), retrieving time and date (`Time`, `Date`), and performing system actions (`restart pc`).

3. **Error Handling and User Interaction:**
   - Handles errors gracefully with exception handling for unrecognized speech (`UnknownValueError`) and service errors (`RequestError`).
   - Maintains user interaction flow with prompts (`Listening...`, `Recognizing...`) and responses (`You said: ...`).

4. **Closest Command Matching:**
   - Uses `difflib` to suggest the closest command match (`get_closest_match()`) when an exact command match isn't found, improving user experience.

5. **Modular Structure and Extensibility:**
   - Organized into functions (`listen()`, `speak()`, `assistant()`) for clear separation of concerns and easy maintenance.

### Example Usage Scenario

The script can be deployed on a desktop or laptop equipped with a microphone. Users can interact with the assistant by speaking commands such as asking for the time, opening applications like Chrome or Epic Games Launcher, or performing system operations like restarting the PC.

### Benefits

- **Accessibility:** Enhances accessibility for users who prefer voice commands over traditional input methods.
- **Convenience:** Provides quick access to information and actions through voice interaction.
- **Customization:** Allows users to add or modify commands based on their specific needs or preferences.

 
