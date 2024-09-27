# Operationalizing Machine Learning

This repository provides the code base for the [HSG CAS Big data & AI for managers](https://cas-bdai.iwi.unisg.ch/) session on how to operationalize machine learning models (September 2024).
All code is based on Azure Machine Learning SDK v2.

## Contents

| Notebook        | Content   |
| ------------- |-------------|
| [0_register_dataset.ipynb](./0_register_dataset.ipynb)      | Registers the csv file as a dataset in Azure ML |
| [1_first_model.ipynb](./1_first_model.ipynb) | Trains a first basic model locally using python's sklearn library.      |
| [2_experiment_tracking.ipynb](./2_experiment_tracking.ipynb) | Re-runs the training process of the previous notebook, this time with tracking model metrics inside Azure ML experiments for traceability purposes. |
| [3_predictions.ipynb](./3_predictions.ipynb) | Sets up a ML pipeline for batch scoring. Loads the previously registered dataset and registered model and generates a CSV file with the models predictions.      |
| [4_deploy_realtime.ipynb](./4_deploy_realtime.ipynb) | Publishes the previously trained model as a REST endpoint in a Microsoft Managed real-time endpoint. This enables getting real-time predictions from the model.      |
| [5_test_ml_endpoint.ipynb](5_test_ml_endpoint.ipynb) | Can be used to send new data via HTTP request to the model endpoint deployed in the previous notebook.

## Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
