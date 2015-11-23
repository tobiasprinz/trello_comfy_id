trello_comfy_id
===============
Comfortable Trello IDs that you can pronounce, are persistent and named helpfully.

Reasoning
---------
If you use Trello cards from a dev perspective, you want them to have a persistent id, so you can name your feature branches. 
Trello cards change their card IDs if you move them from board to board, so these do not work.
 
They should be human-readable to refer them in a conversation. 
Trello links are long and hard to pronounce, so these don't qualify.

Their numbers should be continuously increasing to give a perspective of how old a feature is. 

Implementation
--------------
Uses webhooks. 
Implements a small callback server the Trello hooks into and adds an ID to the title unless given. 
Stores a map of id <-> link.
