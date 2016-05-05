Development dependencies

    npm install vue pug coffee-script watchify vueify browserify browserify-hmr vueify-insert-css vue-hot-reload-api babel-core babel-preset-es2015 babel-plugin-transform-runtime babel-runtime@6 --save-dev

Compile for development (with hot-module-replacement)

    watchify -vd -p browserify-hmr -t vueify -e app/assets/components/index.js -o app/assets/javascripts/components.dev.js
    
Compile for production

    browserify -t vueify -e app/assets/components/index.js -o app/assets/javascripts/components.dist.js
