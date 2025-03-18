<h1>Abstract</h1>
ArtEmotions aims to predict emotional responses to artworks by analyzing features such as art period, artist, creation year, medium, and subject focus. Building upon the WikiArt Emotions dataset, which comprises 4,105 artworks annotated for emotions evoked in observers, this project refines the data and develops a predictive model to classify viewer reactions as positive, negative, or mixed.
<h1>Introduction</h1> 

Art has long been a powerful medium for evoking emotions, with different styles, subjects, and techniques influencing viewers’ reactions in unique ways. Understanding and predicting these emotional responses is a growing area of interest in both psychology and computational analysis. ArtEmotions aims to bridge this gap by developing a predictive model that classifies viewer reactions to artworks as positive, negative, or mixed.

This project builds upon the WikiArt Emotions dataset, a collection of 4,105 artworks annotated with the emotions they evoke in observers (Mohammad & Kiritchenko, 2018). By refining and expanding the dataset, ArtEmotions explores how various artistic features—such as art period, artist, creation year, medium, and subject focus—contribute to emotional perception. Through machine learning techniques, the model seeks to enhance our understanding of the relationship between visual art and human emotion, providing valuable insights for artists, curators, and researchers interested in affective computing and art perception.

This research has broad implications, from improving art recommendation systems to advancing computational aesthetics and emotion recognition in creative works. By quantifying emotional responses to art, ArtEmotions offers a novel approach to analyzing the subjective experience of visual artworks through data-driven methodologies.







<h1>Methods</h1> 

*Data Collection and Cleaning*

The original WikiArt Emotions dataset includes annotations for emotions evoked by artworks, with each piece evaluated by at least ten annotators. Annotations encompass emotions triggered by the image alone, the title alone, and the combination of both, along with ratings on a scale from -3 (dislike) to 3 (like), and indicators of whether the artwork depicts a face or body. For this project, the dataset was refined by:

- Combining separate artist and title columns into a single “artist_title” column for unique identification.
- Consolidating emotion annotations into three categories: positive, negative, and mixed/other.
- Removing columns containing "ImageOnly" and "TitleOnly" data to focus on holistic emotional responses
- Extracting face and body presence into separate binary columns (“Face”, “Body”, “None”)

*Feature Selection*

The predictive model utilizes the following features:
- Art Period: Categorization of the artwork’s historical context.
- Artist: The creator of the artwork.
- Year: The year the artwork was created.
- Medium: Distinguishing between paintings and other art forms.
- Subject Focus: Indicating whether the artwork focuses on a face, body, or neither.

*Model Development*

A Random Forest classifier was developed to predict the emotional response category (positive, negative, mixed) based on the selected features. The dataset was split into training (80%) and testing (20%) sets, and the model was trained to predict emotional responses (positive, negative, mixed). Performance was assessed using accuracy, precision, recall, and F1-score
![image](https://github.com/user-attachments/assets/2ce63f70-d21c-41a7-a8ba-ca9be1341f7e)

<h1>References</h1>
<ol>
  <li>Mohammad, S. M., & Kiritchenko, S. (2018). WikiArt Emotions: An Annotated Dataset of Emotions Evoked by Art. In Proceedings of the 11th Edition of the Language Resources and Evaluation Conference (LREC-2018), Miyazaki, Japan. European Language Resources Association (ELRA).</li>
  <li></li>
</ol>
