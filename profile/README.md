# Archipelago Manager
Manager for [Archipelago](https://github.com/Archipelago-Manager) servers, built for ease of use and increased functionality like configuration management, users, easily host several games, discord integration, notifications etc.
Started as a project because I wanted some easier way to get information about progress while running async games, it then turned into a fully fledged SaaS development project.

Projects is made to be fully open source and self-hostable, but will also serve as a way to learn hosting a SaaS and sold as a service for people who do not want to bother with hosting it themselves.

## Components

#### [archipelago-manager-backend](https://github.com/Archipelago-Manager/archipelago-manager-backend)
Main backend that handles most management, like users, servers, configurations, discord settings etc.

#### [archipelago-manager-node](https://github.com/Archipelago-Manager/archipelago-manager-node)
Backend/node for actual Archipelago servers, this is separated from the backend to allow for easier scaling of these server, for example using kubernetes.
Communication to/from the node API will only be through the backend.

#### archipelago-manager-front-end
Front end client that connects to the back end and allows for management.
Will also include a Text Client to connect to Archipelago servers through the web.

#### archipelago-manager-discord-bot
Discord bot that can connect as a client to a server, to serve messages on server events like item checks and messages.
Will also allow full management of all your servers and users right from discord.
Perfect for a community built around Archipelago!
