# GHA-PublishToAzureStorage
GitHub action for publishing a static site to Azure Storage

## Usage

```yml
 - name: 'Deploy to Azure Storage - mywebsite'
      uses: Shane32/GHA-PublishToAzureStorage@main
      with:
        source-folder: 'reactapp/ClientApp/build'
        storage-account-name: 'myaccount'
        storage-account-connection-string: ${{ secrets.MY_CONNECTION_STRING }}
        container-name: 'public'
        destionation-folder: '/'
```
