# MITDI

Google Drive link to full dataset:
https://drive.google.com/drive/folders/1n9f2Qs_I2KMP5UWlrACfwlhjrLkhPh3d?usp=sharing

Cite Paper:

Chakraborty, N., Mitra, A., Choudhury, A. et al. How to handle bi/tri-lingual Indic texts in a single image? A new dataset of natural scene and born-digital images. Multimed Tools Appl (2022). https://doi.org/10.1007/s11042-022-12596-7

A new dataset called Mixed-lingual Indian Texts in Digital Images (MITDI) is introduced with the following salient features:
1.	MITDI comprises of two sets of images: NSIs and BDIs. In a first of its kind, BDIs with mixed-lingual texts have been introduced.
2.	The current version of this dataset houses images with texts in popular languages like English, Bangla and Hindi. Later versions shall include other Indian languages to present a thorough emphasis on the Indian scenario.
3.	Each image contains texts written in at least two languages along with variations in orientations, fonts, sizes and shades of texts.
4.	Tightly bounded annotations are done at word-level localization and language identification so that precise performance analysis can be made.

Dataset Preparation:
The proposed dataset comprises of two subsets under the name ‘NSI’ for natural scene images and ‘BDI’ for born-digital images, where each subset has 500 images respectively thereby contributing a pool of 1000 images. Here, each individual image has texts in at least two languages among Bangla, English and Hindi.
Annotations are done at word-level since language of any textual content varies from word to word. However, small sized texts are bounded at region-level. Tight word-level horizontal bounding is done such that least amount of non-text region is mapped.
The standard annotation followed is (x,y,wd,ht) where (x,y) is the starting coordinate of the bounding box which is usually the upper left coordinate, wd is the width of the bounding box starting from x coordinate and ht is the height of the bounding box starting from y coordinate.
Each word annotation is labeled as follows: Bangla words are labeled as ‘b’, English words as ‘e’ and Hindi words as ‘h’.

Evaluation Protocol:
The criteria for evaluation on MITDI include the choice of some standard metrics and protocols like Precision (P), Recall (R), F-measure and Accuracy that reflect the quality of performance of any method concerned that are defined as follows:

1. P=TP/(TP+FP)
2. R=TP/(TP+FN)
3. F-measure=(2×P×R)/(P+R)
4. Accuracy=(TP+TN)/(TP+TN+FP+FN)

Where, P and R signify Precision and Recall in Eqs. (1) and (2) respectively.
Also, TP denotes True Positives for pixels within the ground truth text boxes.
The pixels falling outside the ground truth text boxes are considered as True Negatives denoted as TN.
Denoted as FP, False Positives signify pixels wrongly identified as part of the ground truth text boxes and False Negatives, denoted as FN, signify those ground truth text box pixels that are falsely excluded.

Other Papers for Citation:

1. Saha, S., Chakraborty, N., Kundu, S., Paul, S., Mollah, A. F., Basu, S., & Sarkar, R. (2020). Multi-lingual scene text detection and language identification. Pattern Recognition Letters, 138, 16-22. DOI: https://doi.org/10.1016/j.patrec.2020.06.024
2. Chakraborty, N., Kundu, S., Paul, S., Mollah, A. F., Basu, S., & Sarkar, R. (2021). Language identification from multi-lingual scene text images: a CNN based classifier ensemble approach. Journal of Ambient Intelligence and Humanized Computing, 12(7), 7997-8008. DOI: https://doi.org/10.1007/s12652-020-02528-4
3. Chakraborty, N., Chatterjee, A., Singh, P. K., Mollah, A. F., & Sarkar, R. (2021). Application of daisy descriptor for language identification in the wild. Multimedia Tools and Applications, 80(1), 323-344. DOI: https://doi.org/10.1007/s11042-020-09728-2
4. Dutta, I. N., Chakraborty, N., Mollah, A. F., Basu, S., & Sarkar, R. (2021). BOB: a bi-level overlapped binning procedure for scene word binarization. Multimedia Tools and Applications, 80(5), 7609-7635. DOI: https://doi.org/10.1007/s11042-020-09785-7
