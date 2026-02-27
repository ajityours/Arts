# ArtoFact: AI Art Authenticator

Final project for the Building AI course

## Summary

ArtoFact is a computer vision tool designed to support art historians and collectors in verifying the authenticity of paintings. By analyzing high-resolution scans for specific "stylometric" fingerprints—such as brushstroke pressure and edge consistency—the model provides a probability score indicating if a work truly belongs to a specific master’s oeuvre.

![Project Overview](/art-header.png)

## Background

The art market faces growing challenges from sophisticated forgeries and undisclosed AI-generated replicas.
* **Subjectivity:** Traditional authentication relies on human "connoisseurship," which can be prone to error.
* **Market Integrity:** Forgeries devalue cultural heritage and cause significant financial loss.
* **Personal Motivation:** I want to preserve the integrity of human creativity by providing an objective, data-driven "second opinion" for art experts.

## How is it used?

The solution is intended for use by auction houses, galleries, and researchers.
1. **Upload:** A high-resolution photo of the artwork is uploaded to the system.
2. **Analysis:** The AI compares microscopic textures against a verified database of the artist's known works.
3. **Visualization:** The system generates a heatmap showing stylistic inconsistencies.

![User Interface Screenshot](/art-ui-demo.png)

## Data sources and AI methods
The project utilizes deep learning architectures tuned for fine-grained image recognition.
* **Data Sources:** 
    * [The Metropolitan Museum of Art Open Access API](https://www.metmuseum.org)
    * [WikiArt Dataset](https://www.wikiart.org)
* **AI Techniques:**
    * **Convolutional Neural Networks (CNN):** To extract brushstroke patterns.
    * **Heatmap Generation:** To highlight areas that differ from the artist's usual style.


| Feature Analyzed | AI Method |
| ----------- | ----------- |
| Brushstroke Stylometry | ResNet-101 CNN |
| Style Consistency | Transfer Learning |

## Challenges

* **Interpretability:** The AI provides a probability but cannot always "explain" its reasoning in art-historical terms.
* **Data Scarcity:** Rare artists may not have enough authenticated works to build a strong digital fingerprint.
* **Ethics:** There is a risk that forgers could use similar AI to train better forgeries.

## What next?

How could this grow?
* **Mobile App:** A version for on-site verification at small galleries.
* **Hardware Integration:** Combining AI with infrared and X-ray scanners for deeper material analysis.
* **Assistance Needed:** I would need to collaborate with material scientists to integrate chemical pigment data.

## Acknowledgments

* [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org) / [CC BY 2.0](https://creativecommons.org) (Example Image)
* Inspired by the Rembrandt Project and the Building AI course by University of Helsinki.
