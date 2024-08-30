# Optical Character Recognition and Intelligent Character Recognition for Turkish (Graduation Project)

This project involves the development of an OCR (Optical Character Recognition) and ICR (Intelligent Character Recognition) system designed for Turkish handwriting recognition. The project uses TensorFlow and Keras to implement a CNN + LSTM model for recognizing handwritten characters and words.

## Project Overview

This project aims to develop an OCR and ICR system capable of recognizing Turkish handwritten text. The model uses CNN for feature extraction and LSTM for processing sequence data. The training data consists of a dataset containing handwritten characters and words. For the ICR model, handwriting samples were collected from approximately 15-20 different individuals. For the OCR model, words were gathered from digital books available online, encompassing four distinct fonts. Initially, a CNN-based model was tested for letter-based recognition in ICR, but it failed to provide accurate predictions due to the limited dataset. Subsequently, a word-based model with a similar dataset size showed improved performance, leading to the adoption of the CNN+LSTM architecture for both OCR and ICR tasks. This approach has demonstrated better accuracy in recognizing both handwritten and printed text in Turkish, highlighting the effectiveness of the combined CNN+LSTM model in diverse text recognition scenarios.

 **Technologies Used**:
   - Python 3.10.12
   - TensorFlow 2.15.0
   - Keras 3.4.1

Models/
   - 1_Model -> ICR Model for Handwriting Letters
   - 2_Model -> OCR Model for Handwriting Words
   - 3_Model -> OCR Model for Digital Words
     
<br>

- 1_Handwriting_Letters -> Handwriting Letters Test
- 2_Handwriting_Words -> Handwriting Words Test

<hr>

## Results

<table align="center">
  <thead>
    <tr>
      <th>Model</th>
      <th>Character-level Accuracy</th>
      <th>Word-level Accuracy</th>
      <th>Loss</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Model for ICR</td>
      <td>86.85%</td>
      <td>69.45%</td>
      <td>2.1067</td>
    </tr>
    <tr>
      <td>Model for OCR</td>
      <td>68.04%</td>
      <td>55.00%</td>
      <td>1.8430</td>
    </tr>
  </tbody>
</table>


## Conclusion

With the limited database, we have arrived at the following conclusions:

- The ICR model demonstrates higher accuracy at both the character and word levels, reflecting its effectiveness in handling diverse handwriting samples.
- The OCR model performs adequately but shows lower accuracy, emphasizing the need for further improvements in handling printed text recognition.
- If we had access to a larger dataset for the OCR model, we would expect to see higher accuracy, suggesting that more data could significantly enhance its performance.
