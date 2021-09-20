# EC601Project1 Visual Question Answering
## Summary
Visual question answering (VQA) is a computer vision application where a system is given an open-ended question about an image, and the system must respond to its most accurate understanding of its vision, language, and commonsense knowledge. 

## Problem Statement
With emerging technologies for image recognition, language processing and computers preforming tasks at a complex level, human lives can be better with a system that could properly answer questions when asked. VQA is an application that intakes image as an input and use an algorithm to process and generate a natural language answer as an output (2). It is useful in areas where aiding a visually impaired user to navigate a world that is built for the sighted, educating non-native speaker and children on books or games with touch screen and advancing the development of artificial intelligence. 

## Application

According to the World Health Organization, a study has found that at least 2.2 billion people globally have a near of distance vision impairment (4). It is estimated to be four times higher to find people with vision impairment in low and middle-income regions than high-income regions. WHO points out that "young children with early onset severe vision impairment can experience delayed motor, language, emotional, social and cognitive development, with lifelong consequences". The technology of VQA would not only help individuals with blindness -visual acuity worse than 3/60, but it would also help the many including children to continue development and the understanding of visuals. 

To completely solve artificial intelligence, a practical application that is capable of answering general and diverse questions about visual environment is paramount. A powerful artificial intelligence can recognize objects in a scene, understand the relationships and express its knowledge in natural language - typically in a few words or a short sentence. While this task is seemingly trivial for human beings, it requires a computer to comprehend the question and parse through the visual elements in an image (5). VQA is the solution to this purpose where it uses an algorithm or a trained model to extract high-level information from images and perform reasoning based on that information (5). 

## Literature Review
Many literature reviews suggest that VQA is a “multi-discipline AI research problem, involving CV, NLP and Knowledge Representation & Reasoning (KR)” (2). To capture the large range of possibilities within questions and visual environments in real world scenarios, a model must be trained with large dataset of images, questions, and answers. Available datasets where trained models have used are the following:
2)	Microsoft Common Objects in Context (COCO), a dataset with 328,000 images and 2.5 million labeled instances (2). 
2)	Dataset for Question Answering on Real-world images (DAQUAR), a dataset containing 6794 training and 5674 test question-answer pairs that are based on images from the NYU-Depth V2 Dataset (2).
3)	COCO-QA dataset, a dataset with 123,287 images coming from the COCO dataset with 78,736 training and 38,948 testing question-answer pairs (2).
4)	VQA dataset, a dataset that is larger than the COCO dataset, including 50,000 abstract cartoon images (2).
Current approach outline in VQA (2):
1)	Extract features from the question
2)	Extract features from the image
3)	Combine the features to generate an answer based on previous datasets 

Different approaches:
1)	Attention-based approach: setting the focus of the algorithm on the most relevant parts of the input question
  (2)

2)	Bayesian approach: modeling cooccurrence statistics of both the question and the image features to infer relationships between the input question and image (3).

## Open-Source Research 
An example of attention-based approach is the Bottom-Up-Attention model from Peter Anderson and Alessandro Steri on GitHub open source (1). Their code implementations is based on “multi-gpu training of Faster R-CNN with ResNet-101, using object and attribute annotations from Visual Genome”. It used the MSCOCO to win the 2017 VQA Challenge with 70.3% overall accuracy (1). Their expected detection results for the pretrained model are the follow (1):

|  | objects mAP@0.5 | objects weighted mAP@0.5 | attributes mAP@0.5 | attributes weighted mAP@0.5 |
| --- | --- | --- | --- | --- |
| Faster R-CNN, ResNet-101 | 10.2% | 15.1% | 7.8% | 27.8% |

## References
1) Anderson, Peter et al. "Bottom-Up And Top-Down Attention For Image Captioning And Visual Question Answering". Github, 2021, https://github.com/peteanderson80/bottom-up-attention. Accessed 19 Sept 2021.
2) Couto, Javier. "Introduction To Visual Question Answering | Tryolabs Blog". Tryolabs.Com, 2018, https://tryolabs.com/blog/2018/03/01/introduction-to-visual-question-answering/.
3) 3) Singh, Gursimran et al. "A Bayesian Approach To Visual Question Answering". Cs.Ubc.Ca, 2018, https://www.cs.ubc.ca/~saeidnp/files/reports/vqa-bayesian.pdf.
4)  "Vision Impairment And Blindness". Who.Int, 2021, https://www.who.int/news-room/fact-sheets/detail/blindness-and-visual-impairment.
5) "VQA: Vision And Language". Australian Institute For Machine Learning (AIML) | University Of Adelaide, 2021, https://www.adelaide.edu.au/aiml/our-research/machine-learning/vqa-vision-and-language.
