The basic images for creating images of a certain application.

# Usage

* Create a `Dockerfile` in your nodejs application directory with the following content:

  ```
  FROM romson/nodejs

  WORKDIR /app
  ADD . /app
  RUN npm install
  
  ENTRYPOINT ["/nodejs/bin/npm", "start"]
  ```

* Run the following command in your application directory:

  ```
  docker build -t my/app .
  ```
