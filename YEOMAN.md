export NPM_PACKAGES="/Users/mariohmol/.npm-packages"
export NODE_PATH="$NPM_PACKAGES/lib/node_modules${NODE_PATH:+:$NODE_PATH}"
export NODE_PATH="/Users/mariohmol/.npm-packages/lib/node_modules"
export PATH="$NPM_PACKAGES/bin:$PATH"
export NODE_PATH=$HOME/.npm-packages/lib/node_modules/


Make sure that /usr/local/bin is in your $PATH.
npm -g root
export NODE_PATH=/usr/local/lib/node_modules
npm rebuild

rm -rf node_modules
rm package-lock.json
npm cache clear --force
npm rebuild
npm i