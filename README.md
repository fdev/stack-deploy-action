# Stack Deploy Action :rocket:

Triggers a deploy of an app on a Stack server. 

## Usage

```yaml
- uses: fdev/stack-deploy-action@v1
  with:
    app: myappname
    ssh-key: ${{ secrets.STACK_SSH_KEY }}
```

## Inputs

| Name      | Description                                    |      Required      | Default value     |
|-----------|------------------------------------------------|:------------------:|-------------------|
| `app`     | Name of the app.                               | :heavy_check_mark: |                   |
| `server`  | Stack server where the app should be deployed. |        :x:         | `'stack.fdev.nl'` |
| `ssh-key` | Private SSH key used to connect to the server. | :heavy_check_mark: |                   |
