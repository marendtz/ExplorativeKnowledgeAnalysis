<br />
<div align="center">

<h3 align="center">Explorative Knowledge Analysis</h3>

  <p align="center">    
    <a href="https://pytorch.org/">Pytorch</a>
    ·
    <a href="https://huggingface.co/docs/transformers/index">Transformers</a>
  </p>
</div>


<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project (Research Proposal)</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



## About The Project (Research Proposal)

This repository offers a simple setup of a 2 layer decoder model for generation.
The model is trained on simple integer sequences and generates the sequence moved one step to the right, where the new element is the class label of the sequence.
Additional class methods allow the extraction of model states (attention output, feed forward output) and the fixure of certain model intermediate states.
This allows for the implementation of causal analysis methodd, which is used to investigate the model's behaviour in case of e.g. knowledge conflicts.

Each jupyter notebook can be run in a virtual environment, which is set up in the following steps.
Noteboos are:
  * Model Modules: Contains the model architecture: ``./src/model_basic/modules.ipynb``
  * Model Training: Contains the generation of synthetic data and the training: ``./src/model_basic/train_model.ipynb``
  * Embeddings Analysis: Contains the analysis of the model's generated embeddings of position and token: ``./src/model_basic/analysis_embeddings_tokens.ipynb``, ``./src/model_basic/analysis_embeddings_positions.ipynb``
  * Analysis of inner states: Contains the analysis of the model's inner representations: ``./src/model_basic/analysis_inner_representation.ipynb``
  * Causal Analysis: Contains the causal analysis of the model's inner representations: ``./src/model_basic/causal_analysis.ipynb``


<p align="right">(<a href="#readme-top">back to top</a>)</p>



## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

0. Clone the repo
   ```sh
   git clone ...
    ```

1. Install virtual environment manager
   ```sh
   pip install virtualenv
   ```

2. Create & activate environment for this project
   ```sh
    virtualenv venv
    source venv/bin/activate
    ```

3. Install kernel and jupyter notebook
    ```sh
    pip install ipykernel 
    pip install notebook
    ```

4. Generate and activate a jupyter notebook kernel and jupyter notebook
    ```sh
    python -m ipykernel install --user --name=venv
     ```

5. Install further project specific dependencies
    ```sh
    pip install -r requirements.txt
     ```

6. Start jupyter notebook
    ```sh
    jupyter notebook
     ```

### Usage

(tbd)


<p align="right">(<a href="#readme-top">back to top</a>)</p>



## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## Acknowledgments

* https://peterbloem.nl/blog/transformers + https://github.com/pbloem/former (MIT License)


<p align="right">(<a href="#readme-top">back to top</a>)</p>


