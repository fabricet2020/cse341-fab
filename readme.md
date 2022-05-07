# How to run it

Run npm install and npm start from the backend folder in the terminal

Test the endpoints in the routes.rest file with Rest Client or another similar tool.

### Video

[Video Example for Students without showing all code](https://youtu.be/0iVptecZ0-E)

# Installing Linters

# 1. Install VS Code extensions

    ESLint
    Prettier Code Formatter

    After the installations press ctrl + , (control + comma)

    Search for 'format on save'
    And make sure Format on save is checked
    (Which will changes double quotes to singles quotes, force semi-colons to exist,...)

    Search for Prettier
    Check the settings for Single Quote

# 2. Install the Prettier plugin and config

    npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
    npx install-peerdeps --dev eslint-config-airbnb

# 3. Create a config file

    .prettierrc

    and type the prettier rules:
    {
        "semi": true,
        "tabWidth": 2,
        "printWidth": 100,
        "singleQuote": true,
        "trailingComma": "none",
        "jsxBracketSameLine": true
    }

    .eslintrc.json
    You cn do it manually or install it globally type:

    sudo npm i -g eslint OR npm install eslint --save-dev
    eslint --init OR npm init @eslint/config

    have these typed
    {
    "extends": ["airbnb", "prettier"],
    "plugins": ["prettier"],

    "rules": {
    }

}

Need to be installed as well
npm i -S body-parser

# 4. Testing

    These 3 lines need to be added in our package.json under script

    "lint": "eslint .",
    "lint:fix": "eslint --fix",

    "format": "prettier --write ./**/*.{js,html}" //Works for me


    "format": "prettier --write './**/*.{js,jsx,ts,tsx,css,md,json}' --config ./.prettierrc"

# Use Swagger tools build your APIs and the OpenAPI specification to describe your APIs

    Add the
    npm install --save-dev swagger-autogen
    npm install cors
    npm install swagger-ui-express
    npm install mongoose

# install

npm install joi-password-complexity
