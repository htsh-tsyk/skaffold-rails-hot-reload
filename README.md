### Example: hot-reload with Ruby on Rails

Application demonstrating the file synchronization mode with Ruby on Rails.

#### Init

```bash
skaffold dev
```

#### Workflow

* Make some changes to `src/rails-sample/app/controllers/welcome_controller.rb`:
    * The file will be synchronized to the cluster
    * `puma` will restart the application
