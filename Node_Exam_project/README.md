# Goal
Exam project by Freja Johannessen for Node fullstack. The project is meant to be a platform for deck creation in the card game Magic the gathering. Nice to have is calling scryfalls api, to get updates on new cards and prices, whilst upholding their rate limits.
## Feature requirements
An app where a user can create decks and add cards to those decks. I wish to:
### Must have
- A card with its details to be displayed
- A deck where cards can be added to
- A user to be saved, with data such as decks
- A filereader that can read data from a JSONL and gziped file
- A search engine for cards, when adding a card
### Nice to have
- An api client that calls scryfalls api for bulkfiles (following their ratelimits and useragent requirements)
- Api client can call scryfalls manifest to check for image updates (scyfall is changing image format from jpeg to webP using a slow rollout). A util should then compare to existing database and call scryfalls other api for indeviedual card changes
## project structure
- public contains public parts like images, and clientside scripts
- resources contain JSONL gziped files, that contain card information
- src contains the template engine components to be used by svelte
- utils contains serverside utility scripts, like a filereader for the card file, and the api client that may be implimented
## Author Freja Johannessen