# concourse-demo-app

## steps for a quick demo environment


- **install concourse**

  ```
  $ vagrant init concourse/lite; vagrant up --provider virtualbox
  ```

- **get demo app**

  ```
  $ git clone git@github.com:xchapter7x/concourse-demo-app.git
  ```

- **setup your creds**(modify file contents)

  ```
  $ cp ci/credentials.yml.sample ci/credentials.yml
  ```

- **add / update your pipeline into your local concourse**

  ```
  $ ./update_pipeline
  ```

- **run some unit tests against your local concourse**

  ```
  $ ./run_units
  ```
