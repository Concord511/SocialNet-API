# SocialNet-API

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)
- [Tests](#tests)
- [Questions](#questions)

## Description

This project is a sample back-end for a social media site. It can create users, their thoughts, and reactions to those thoughts. It can also create a friends list.

## Installation

You will need express and mongoose.

## Usage

API calls are made as follows:

### User Routes

localhost:3001/api/users

- getAllUsers
- createUser

        JSON: {
            "username": "<desiredUsername>",
            "email": "<desiredEmail>"
        }

localhost:3001/api/users/:id

- getUserById
- updateUser

        JSON: {
            "username": "<desiredName>",
            "email": "<desiredEmail>"
        }

- deleteUser

localhost:3001/api/:usersId/:friendId

- addFriend
- removeFriend

### Thought Routes

localhost:3001/api/thoughts

- getAllThoughts
- createThought

        JSON: {
            "thoughtText": "<thoughtText>",
            "username": "<userName>",
            "userId": "<userId>"
        }

localhost:3001/api/thoughts/:id

- getThoughtById
- updateThought

        JSON: {
            "thoughtText": "<thoughtText>",
            "username": "<userName>",
            "userId": "<userId>"
        }

- deleteThought

localhost:3001/api/thoughts/:thoughtId/reactions

- createReaction

        JSON: {
            "reactionBody": "<reactionText",
            "username": "<userName>",
            "userId": "<userId>"
        }

localhost:3001/api/thoughts/:thoughtId/:reactionId

- deleteRaction

## License

This project is covered under the Unliscensed license:

## Contributing

Contributions welcome, but not necessary.

## Tests

Insomnia Core used to confirm all routes functioning as intended.

## Questions

Find me on GitHub: https://github.com/Concord511

Email me with questions: concord511@gmail.com
