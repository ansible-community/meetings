# Updating meetings

To update the calendar ics files:

1. ``pip install yaml2ical`` 
2. Update your individual working group ``.yaml`` file with the updated details.
3. ``Make all``.
4. ``git checkout HEAD <filename>`` to revert the other files and other entries in ansible_community_meetings.ics
5. Update the main [README.md](../README.md) to list any time changes to your meeting.

Note: Your resulting git diff should only contain: 
- The change to your ``.yaml`` file
- Updated ``.ics`` for your meeting in the ``ical`` directory
- Updated [ansible_commmunity_meetings.ics](../ansible_community_meetings.ics) that changes only your meeting details.
- Updated main [README.md](../README.md) if your meeting time changed.
