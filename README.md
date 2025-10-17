# Unhinged Therapist Dataset

This repository contains a curated dataset of fictional conversations between a patient and their "unhinged" therapist. The therapist's responses are designed to be unconventional, humorous, and thought-provoking, falling into categories like dark comedy, sarcasm, and absurdism. This dataset is intended for creative and research purposes, such as training language models, analyzing conversational AI, or simply for entertainment.

## Dataset Structure

The dataset is provided in a single CSV file: `dataset.csv`.

The file has the following columns:

*   `patient_inquiry`: The patient's statement, question, or concern.
*   `therapist_response`: The therapist's unconventional and "unhinged" response.
*   `tone_label`: A label classifying the tone of the therapist's response.

### Tone Labels

The following tone labels are used in the dataset:

*   **sarcastic**: Dry, witty, and often ironic responses that mean the opposite of what is literally said.
*   **dark comedy**: Humor that makes light of serious, disturbing, or taboo subject matter.
*   **absurdist**: Responses that are illogical, nonsensical, or surreal in a humorous way.
*   **blunt**: Brutally honest, direct, and straightforward responses without any sugar-coating.
*   **passive-aggressive**: Indirect expressions of negative feelings, resentment, or aggression.

## Example

Here is an example row from the dataset:

| patient_inquiry                                                                                             | therapist_response                                                                                                                            | tone_label |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| "I've been feeling like I'm constantly letting everyone down. I try so hard, but someone always seems disappointed." | "Maybe stop auditioning for roles nobody asked you to play. You’re not the main character in everyone’s tragedy. Try letting someone else be disappointed for once." | sarcastic  |

## Contributing

Contributions are welcome! If you have ideas for new conversation examples, new tone categories, or improvements to the existing data, please feel free to open an issue or submit a pull request.

When contributing, please ensure that new entries follow the existing CSV format and that the tone labels are consistent with the definitions provided above.

## Disclaimer

This dataset is a work of fiction and is intended for entertainment and research purposes only. The conversations depicted are not representative of actual therapeutic advice or practice. The content is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.
