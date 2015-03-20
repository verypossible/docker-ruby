# Spartan Docker Ruby

This image provides Ruby and Bundler. On the build of the image, it adds your `Gemfile` and `Gemfile.lock` to `/app/`, runs `bundle install`, and adds the application code to the `/app` directory.

## Usage

1. Add the file `start_services.sh` to the `deploy` directory in the application root directory. This script is executed when the container is started without a command.
2. Ensure your application binds to port `3000`.
3. Set up a `Dockerfile` with the following contents:

    ```
    FROM spartan/ruby
    ```
4. Build the image.
5. …
6. Profit.
