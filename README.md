Library Documentation: Improved AFK Detection for SAMP
Description:

This library provides functionality for detecting AFK (Away From Keyboard) players in San Andreas Multiplayer (SA:MP). It tracks player activity and pauses/unpauses them accordingly based on inactivity.
Usage:

    Include the library in your Pawn script.
    Implement the callbacks OnPlayerPause and OnPlayerUnpause to handle player pausing and unpausing events.
    Optionally, utilize functions IsPlayerPause and TimeSincePaused to retrieve AFK status and time since pausing, respectively.

Functions:

    IsPlayerPaused(playerid);
        Description: Checks if the player is currently paused.
        Parameters:
            playerid: ID of the player.
        Returns: 1 if the player is paused, 0 otherwise.

    TimeSincePaused(playerid);
        Description: Retrieves the time elapsed since the player was paused.
        Parameters:
            playerid: ID of the player.
        Returns: Time elapsed (in seconds) since the player was paused.
Callbacks:

    public OnPlayerPause(playerid) {
      // Your code here
    }

    public OnPlayerUnpause(playerid) {
      // Your code here
    }

Notes:

    This library is optimized for use with San Andreas Multiplayer (SA:MP) servers.
    Ensure that callbacks OnPlayerPause and OnPlayerUnpause are properly implemented to handle player pausing and unpausing events.

README:
Improved AFK Detection for SAMP

This library provides enhanced AFK (Away From Keyboard) detection functionality for SA:MP servers. It automatically detects inactive players and pauses them, triggering the appropriate events for handling AFK status changes.
Installation:

    Copy the iafk.inc file into your SA:MP server's pawno/includes directory.
    Include the library in your Pawn script using #include <iafk>.

Usage:

    Implement the required callback functions: OnPlayerPause and OnPlayerUnpause.
    Utilize the provided functions to check AFK status and time since pausing, if needed.

Credits:

    Original Credits to Miihai
    Improved by realdiegopoptart for compatibility with YSI foreach.

License:

This library is provided under the MIT License. Feel free to modify and distribute it as needed.
