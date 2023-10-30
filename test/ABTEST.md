## AB Test Name: Landing Page

**User Story Number:**  8

**Metric:** Average time spent on the landing screen (between the screen opening and closing), measured in seconds

**Hypothesis:** Conventionally, the landing screen of a social app is a mishmash of UI elements organized and resized to suit the needs of the average user, similar to widgets. The purpose of a landing screen is to predict a handful of things the user is most likely to do or navigate to, and present shortcuts to them. This is meant to prevent the user from searching and navigating through the app unnecessarily. Right now, the landing page contains a "join club" button, a "create club" button, and a list of clubs the user is a member of, the sizes of which might be detracting from the convenience of the screen. The elements need to be sized proportionally to their relative importance – large enough to view easily, but small enough to give the other elements breathing room. I hypothesize that giving each club list item a width:height aspect ratio of 2:1 will decrease the average time spent on the loading screen more than any other such ratio, including the current ratio of 33:13.

**Experiment:** I will use Firebase's built-in AB testing capability, using the club list item aspect ratio as the sole parameter in the remote config panel. 5% of the user base will be randomly allocated to this experiment. This percentage is intentionally low because I don't want to risk alienating a signficant fraction of the user base due to a glitch or offensive implications in any of the variations. The default value of the parameter will be 33:13.

**Variations:** The first variation will have an aspect ratio value of 2:1, a satisfyingly simpler decrease from the default value. The second variation will have an aspect ratio of 33:5, an increase from the default that would limit the club list item to just the club name.

## AB Test Name: Color Scheme (James) 

**User Story Number:**  9

**Metric:** Time on app per day per week

**Hypothesis:** The color scheming of an app can greatly alter the user experience. Colors have a subconscious affect on how much a user can enjoy using the app. Currently, our app has a green color scheme to reflect the outdoors. Our current color scheme involves the colors DDE392, AFBE8F, 7D8570, 646F58, and 504B3A. I hypothesize that using the colors 313268, 595358, 857F74, A4AC96, and CADF9E will decrease the average time on the app per day per week because it is using more modern and professional colors, but lacks the nice coherency of the first set of colors.

**Experiment:** I will use Firebase's AB testing to allocate 5% of our userbase to have the new color scheme of 313268, 595358, 857F74, A4AC96, and CADF9E. Only 5% of our users will experience the change so that the majority of our userbase will not be affected by the experimental change. By tracking the average time on our app per day per week, we can see how the new color scheme performs in comparison to the old one.

**Variations:** The "A" variation of our app will have the color scheme DDE392, AFBE8F, 7D8570, 646F58, and 504B3A. The "B" variation of our app will have the color scheme 313268, 595358, 857F74, A4AC96, and CADF9E.

