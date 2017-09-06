Twitch Viewers and Followers
============================

Hypothesis
----------

1. "Big channels" have more followers and more viewers than do "small channels", and gain viewers at a greater rate.
2. However, these rates differ for different categories - eg Creative vs Gaming vs IRL.
3. With a baseline established, statistical outliers can be recognized and explored.

Data collection
---------------

1. Probe a number of channels for their viewer counts (must be online??) and follower counts.
2. Query the channel's 100 most recent followers. Look at the 100th and subtract its created_at from now. This gives a "time for 100 follows".
   - If there are less than 100 followers, "no data". Don't try to extrapolate from too few results.
   - To keep everything on the same kind of scale (bigger channel wants higher numbers), yield 604800/x to give the average viewers per week.
3. Query the channel's 100 most recent archived videos. Categorize the channel by the "game" given.
   - If there aren't 100 followers, use whatever we have, as long as it's at least, say, 5 videos.
   - The game given won't necessarily reflect the entire stream, as it can change. It does seem to pick the majority though.
   - Some Creative streamers use IRL while being creative. Can I get the communities used during the stream??
