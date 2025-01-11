# Stack Deploy Action :rocket:

Triggers a deploy of an app on a Stack server. 

## Usage

```yaml
- uses: fdev/stack-deploy-action@v1
  with:
    app: myappname
    server: myserver.com
    services: http mail
    ssh-key: ${{ secrets.STACK_SSH_KEY }}
```

## Inputs

| Name       | Description                                    |      Required      |
|------------|------------------------------------------------|:------------------:|
| `app`      | Name of the app.                               | :heavy_check_mark: |
| `services` | Services to deploy (separated by spaces)       |        :x:         |
| `server`   | Stack server where the app should be deployed. | :heavy_check_mark: |
| `ssh-key`  | Private SSH key used to connect to the server. | :heavy_check_mark: |
