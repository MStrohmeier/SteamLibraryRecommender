# SteamLibraryRecommender
A utility that examines your Steam library and suggests games you already own that you might enjoy playing.

Deadline: May 4, 2015

This tool will use an AI tuned using machine learning techniques to examine your library, see what sort of games you enjoy, then suggest other games you already own that you might want to play. The algorithm will likely be inspired by that used by the Netflix prize entrants, though with a focus on gameplay time instead of ratings. User tags, if possible, will drive the recommendation system. Failing that, the system may have to draw correlations between gameplay time of a large sample of users.

Initial thoughts are to take a logarithmic function of number of hours played on each game, find the average value per tag of this function, then return games that have unusually low gameplay time. The system will learn how to weight tags based on how long a typical user plays that type of game; RPGs might expect to see much greater playing time than, for instance, casual games. The system should also more heavily weight tags that match games the user has played a lot of recently, as this might represent a shift in the user's game choices. Other possible attributes to consider include average time on specific games across all Steam players or ratings for a game, but these will be secondary to the user's specific preferences.

At this time it is not clear which language will best suit this project or how the final results will be presented to the user. Challenges will include learning how to best use the Steam API, learning an appropriate database or other storage structure for data, and getting enough training data to hone the system. Having just 30 days to complete this project will also pose a substantial risk.
