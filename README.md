# ts-starter-template
Simple starter template for typescript projects (prettier, eslint, tsconfig etc.)

# Requirements
- An enviroment with nodejs (recommend latest lts)
- Yarn version >= 1.22.0 && < 2.0.0
    - Install yarn using these instructions https://classic.yarnpkg.com/en/docs/install/
- PowerShell 7 (used to clean up dist before build)
    - Install using these instructions https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.3
- Understanding of typescript

# Setup & Development
1. Click on the big green button or [here](https://github.com/Pepijn98/ts-starter-template/generate)
    - Create your new repo using this template
    - Clone the repo locally using `git clone https://github.com/USERNAME/REPO.git`
        - If you're using ssh you can also use `git clone git@github.com:USERNAME/REPO.git` instead
2. Make sure to uncomment `.env` in `.gitignore` before pushing anything
3. Run `yarn install` to install the dependencies
4. Basic commands
    - `yarn deploy` to start it using pm2 (usefull for keeping a process running on a vps)
        - if you don't have pm2 install it using `npm i -g pm2`
    - `yarn start` to run the production version
    - `yarn test` to run the development version using generated javascript
    - `yarn dev` to run the development version using ts-node
    - `yarn build` generates the production javascript files in `./dist`
    - `yarn build-test` runs the same command as `yarn build` without generating any files
    - `yarn clean` removes `node_modules` and `yarn.lock`
    - `yarn lint` check all typescript files using eslint
    - `yarn lint-fix` fix all typescript files using eslint

**Before using `yarn deploy` you have to run `yarn build` first to generate the javascript files.**

## Support
[![discord](https://discordapp.com/api/v6/guilds/240059867744698368/widget.png?style=banner2)](https://discord.gg/qqtrrMj)
