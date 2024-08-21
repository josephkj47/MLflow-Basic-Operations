# MLflow-Basic-Operations


## For Dagshub

https://dagshub.com/josephkj47/MLflow-Basic-Operations.mlflow

import dagshub
dagshub.init(repo_owner='josephkj47', repo_name='MLflow-Basic-Operations', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

  MLFLOW_TRACKING_URI=https://dagshub.com/<username>/<repo>.mlflow python3 <file-name>.py
