# IrcAutosuggest
Autosuggest for a chat client

This script retrieves top 10 users and channels that start with a string 
(auto-complete) for a user. It determines the order using frecency. The data
structure used is a trie for fast retrieval.

Input format:
It reads in a user's historical interactions where each row is of the form
(channel/user, timestamp). It also reads in all channels in an organization
independent of whether a user has visited those channels in the past or not.
That file is just a list of channel names. Example files are provided.
