# rails-vue

rails-vue adds support for vue components (`.vue` files) to rails. In development environment, it provides hot-reloading of components via browserify-hmr. In production, it compiles them to CSS and JS during the asset compile step.

# Get started

First, install the development dependencies

    npm install watchify vueify browserify browserify-hmr vueify-insert-css vue-hot-reload-api babel-core babel-preset-es2015 babel-plugin-transform-runtime babel-runtime@6 --save-dev

Add the gem to your Gemfile (doesn't exist yet).

    gem 'rails-vue'
    
Now you can place your `.vue` components into `app/assets/components`.

That's it.
