# How to submit

## Labels

Here we present the rules of how we expect the community to use labels to enforce a standardized experimental protocol for easy and direct model comparison:

-   **Training labels**: Training model parameters (can be used in whatever ways, e.g., for gradient-descent, model input).  
    
-   **Validation labels**: Meant for standard hyper-parameters tuning (not allowed: gradient-based search, use as model input).  
    
-   **Test labels**: Final model evaluation.

## Submissions

Our public leaderboards are meant to allow researchers to showcase and keep track of state-of-the-art methods and encourage reproducible research. To appear on a leaderboard, a new method must follow the experimental protocol mentioned above and be submitted along with the following information.

### Required information

-   **OCPSB package version**: OCPSB PyPi package version used.
-   **Method**: Name of the method.
-   **Dataset**: Name of an OCPSB dataset that you use to evaluate the method.
-   **Test performance**: Raw test performance output by OCPSB model evaluators.
-   **Validation performance**: Validation performance of the model that is used to report the test performance above.
-   **Code**: The link to a Github repository or directory containining all code to reproduce the result. **A placeholder repository is not allowed.**
    -   The authors are responsible for addressing any inquiry about their code.
    -   **Please add `README` and provide enough instruction (i.e., exact command) to reproduce the submitted result.**
-   **Paper**: The original paper describing the method (arXiv link is recommended. paper needs not be peer-reviewed). If your method has any original component (e.g., even just combining existing methods XXX and YYY), you have to write a technical report describing it (e.g., how you exactly combined XXX and YYY).
-   **Tuned hyper-parameters**: Please kindly disclose all the hyper-parameters you tuned, and how much you tuned for each of them. Please follow the following form: `"lr: [0.001*, 0.01], num_layers: [4*,5], hidden_channels: [128, 256*], dropout: [0*, 0.5], epochs: early-stop*"`, where the asterisks (\*) denote the hyper-parameters you eventually selected (based on validation performance) to report the test performance. This information will not appear in the leaderboard for the time being, but it is important for us to keep the record and encourage the fair model selection.
-   **Hardware**: The hardware (primarily for GPU) used for the experiments, e.g., GeForce RTX 2080 (11GB GPU). If multiple GPUs are used, please specify so.
-   **Officiality**: Whether the implementation is **official** (implementation by authors who proposed the method) or **unofficial** (re-implementation of the method by non-authors).

### Submit

Once you have developed and evaluated a new method, please use our [email template](mailto: imb-benchmark@hsu-hh.de) to send us all information mentioned above.
Results will be added to the respective leaderboard once we have checked their validity. 

**Note:** We will only publish reproducible submissions including all necessary information. Please [contact us](mailto: imb-benchmark@hsu-hh.de) if there is anything unclear or you have found any problematic submission on the leaderboards.
