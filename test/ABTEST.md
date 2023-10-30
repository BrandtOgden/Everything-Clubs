## AB Test Name: Landing Page

**User Story Number:**  31

**Metric:** Average time spent on the landing screen (between the screen opening and closing), measured in seconds

**Hypothesis:** Conventionally, the landing screen of a social app is a mishmash of UI elements organized and resized to suit the needs of the average user, similar to widgets. The purpose of a landing screen is to predict a handful of things the user is most likely to do or navigate to, and present shortcuts to them. This is meant to prevent the user from searching and navigating through the app unnecessarily. Right now, the landing page contains a "join club" button, a "create club" button, and a list of clubs the user is a member of, the sizes of which might be detracting from the convenience of the screen. The elements need to be sized proportionally to their relative importance – large enough to view easily, but small enough to give the other elements breathing room. I hypothesize that giving each club list item a width:height aspect ratio of 2:1 will decrease the average time spent on the loading screen more than any other such ratio, including the current ratio of 33:13.

**Experiment:** I will use Firebase's built-in AB testing capability, using the club list item aspect ratio as the sole parameter in the remote config panel. 5% of the user base will be randomly allocated to this experiment. This percentage is intentionally low because I don't want to risk alienating a signficant fraction of the user base due to a glitch or offensive implications in any of the variations. The default value of the parameter will be 33:13.

**Variations:** The first variation will have an aspect ratio value of 2:1, a satisfyingly simpler decrease from the default value. The second variation will have an aspect ratio of 33:5, an increase from the default that would limit the club list item to just the club name.

## AB Test Name: Color Scheme (James) 

**User Story Number:**  

**Metric:**
**Hypothesis:**

**Experiment:**

**Variations:**

