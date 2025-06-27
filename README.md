# 2025-1A-T02-G84-PUBLICO
Repository for group 84 of class T02 (2025/1A)

# Public Report - Empreendedorismo  
**Inteli - Instituto de Tecnologia e Liderança**  
Avenida Professor Almeida Prado, 520, Butantã, São Paulo, SP  
CEP: 05508-070  
[www.inteli.edu.br](http://www.inteli.edu.br)  

---

## 1. Project team members  
- **Antônio Ribeiro Cavalcante**  
- **Yasmin Vitória Rocha de Jesus**

## 2. Introduction The Leap to Q2

**From a Validated Idea to an MVP that Already Identifies Libras Signs**

After demonstrating social relevance and business potential in the **first quarter**, we spent the **second quarter** giving technical shape to the project. We built a prototype that recognizes the Libras alphabet in real time and establishes the foundations for gesture expansion, image storage, and continuous learning with deep learning.

---

| **Q1**                                                  | **Q2**                                                                                                        |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Problem diagnosis, market validation, and B2B strategy. | MVP construction: functional algorithm, instant feedback, image storage, and groundwork for future expansion. |

In just a few months, the project evolved from a conceptual proposal to a functional prototype capable of recognizing Libras letters live on camera. This was achieved by developing a complete computer-vision pipeline that combines convolutional neural networks (CNNs), hand-landmark vectorization via MediaPipe, and instant user feedback.

To ensure continuous model improvement, we implemented an **image bucket** that automatically stores each captured gesture. The bucket serves two purposes: it lets users review their attempts and feeds real-world data back into the AI, steadily boosting accuracy.

Reaching this stage required rigorous technical decisions—testing multiple neural-network architectures, tuning performance, and discarding approaches that would not scale. The results prove that Libras training can become part of everyday corporate life through accessible, efficient technology. We now move on to dynamic gestures—gaps with proposed solutions already mapped—and more robust validation, paving the way for an even more complete, contextualized solution.

---

## 3. Module Objective

We delivered a usable prototype that:

1. **Captures hand gestures** through a webcam.
2. **Identifies the letter** being signed.
3. **Displays the result** on-screen within seconds of the gesture.
4. **Stores every gesture** in a dedicated bucket, eliminating the need for external image APIs and enabling continuous reuse.

---

## 4. Path Taken

| **Step**            | **What We Did**                                                     | **Why It Matters**                                                                                     |
| ------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **Data collection** | Tested multiple datasets and diagnosed improvement points.          | High-quality, varied examples are essential—poor datasets are a major gap in sign-language technology. |
| **Model testing**   | Compared MLP, RNN, and CNN approaches.                              | Ensured we chose the most stable and production-ready option.                                          |
| **CNN selection**   | Achieved the best balance of accuracy and speed.                    | Fewer attempts needed to “get” the gesture, thanks to high letter-detection rates.                     |
| **Image bucket**    | Implemented an AWS S3 bucket for training images and user captures. | Images are visible in the frontend and fuel model-improvement cycles.                                  |

---

## 5. Results

* **Live operation:** Users sign a letter and see the recognized result in under one second.
* **Accuracy:** \~97 % correct detections, even with imperfect lighting.
* **AWS bucket:** Users select a letter, which is fetched via a dedicated API so they can repeat it.
* **Gamified feedback:** Currently the system shows the detected letter; future versions will add messages like “Good job!” or “Try again,” add points, and motivate learning.

---

## 6. Lessons Learned

1. **Data diversity:** More angles, hands, and settings are needed; data-augmentation techniques and the bucket make this feasible.
2. **Experience over numbers:** Usability drove every decision. Testing until we found the right model avoided forcing users to repeat gestures or mislabeling correct signs—issues that surfaced in early versions and can derail engagement.
3. **Libras is movement:** The alphabet is only the entry point; we must now incorporate more complex gestures, full words, and phrases.

---

## 7. Next Steps

| **Next Step**                    | **Description**                                                                               |
| -------------------------------- | --------------------------------------------------------------------------------------------- |
| **Expand the dataset**           | Use the bucket to collect short videos (≈ 3 s) of dynamic gestures in real settings.          |
| **Dataset variation**            | Add avatar-based images to diversify hand shapes and improve recognition accuracy.            |
| **Corporate API**                | Provide an endpoint that accepts frames, returns feedback, and stores captures in the bucket. |
| **Generative AI for user input** | Allow users to type a word and see its Libras translation rendered live on screen.            |

---

## 8. Conclusion

The results in this module confirm the **technical feasibility** of our approach: the prototype already recognizes the entire Libras alphabet in real time and stores each gesture for continuous model feedback. However, the MVP is still experimental—datasets must grow, dynamic gestures must be integrated, performance metrics refined, and user experience validated in real corporate settings with testers. With these improvements, we will evolve from a promising prototype into a truly scalable Libras-training platform, capable of delivering business value while reducing communication barriers across the workplace.





