Team members: Makda Dejene, Sively De Los Santos, Kambinachi Obioha

File Descriptions
 
- reddit_classification.ipynb: Main notebook. Trains two CNN models on manually labeled photo crops: one classifying who is in the frame (selfie, solo, group) and one classifying the context (outdoors, gym, everyday, etc.). Also runs inference and writes predictions back to the posts JSON.
- crop_labels_manual.csv: Manual annotations for each photo crop. Contains three columns: filename, person label, and context label.
- profile_review_posts_real(1).json: Scraped posts from r/hingeapp. Each entry includes the post metadata, images, community comments, and the model's predicted person and context labels per crop.
- Final_Sentiment_Analysis.ipynb: Uses VADER to score comment sentiment per post, then aggregates average sentiment by person category, context category, person-context combinations. This also contains the visualization as it outputs bar charts, confusion matirx, and heatmap
- hingeapp_crops: folder containing cropped images scrapped from reddit, with corresponding labels to crop_labels_manual.csv and profile_review_posts(real)(1)
