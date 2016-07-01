# makenv

A handy set of tools for creating and using .env files

## makenv

Use `makenv` to build up a `.env` file. It will prompt you for a variable name followed by it's value. When finished, leave the variable name blank and hit Enter to write the file. The file's contents will be shown at the end.

## dotenv

Use `dotenv` to pass the contents of your `.env` file into the command that follows.

For example, lets say your `.env` file contained:

    PORT=3000
    NODE_ENV=production

If you ran the following

    dotenv docker-compose up

It would expand to

    PORT=3000 NODE_ENV=production docker-compose up
