# Remix vs NextJS

Update this with your project details as you go.

# What is this demo?

Remix and NextJS are frameworks for building web applications with React both popular server-side rendering (SSR) both are supported for deploy on Vercel.

# How do you run it?

Use node at least version 16

Create a .env file with the following values:

| Variable          |   SQLITE      |  POSTGRESQL                                   |
|:------------------|:--------------|:----------------------------------------------|
| DATABASE_PROVIDER | sqlite        | postgresql                                    |
| DATABASE_URL      | file:dev.db   | postgresql://USER:PASSWORD@HOST:PORT/DATABASE |
| SESSION_SECRET    | something     | something                                     |

Install dependencies:

`npm install`

In the scripts there is a `postinstall` script that will create the db and seed it.

But if for some reason you want to setup and seed the database manually, run:

```
npx prisma db push
npx prisma db seed
```

Start the application on port `3000`

```sh
npm run dev
```

If you want to play around with a logged user, you can register yours or use the seed one

```
user: kody
pwd: twixrox
```

# Understand
### What competitors are there?

- Gatsby
- Create React App (although it is no longer suggested)

### Why would this be any different than the competition?

- NextJS is backed up by Vercel and more than 2.6K contributors
- Remix has more than 500 contributors.

# Conclude
### Would you recommend using this technology in the future?

- Definitely both frameworks provide very useful features to run react components and are easy to understand once you got the basics.

### What situations would it be more useful than the competitors?

- Remix provides a more browser like experiences where you have the full control of the browser properties. While NextJS provides a more robust application structure for more complex projects.
