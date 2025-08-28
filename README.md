# Real-Time Object Detection with YOLO + VLM

This project demonstrates real-time object detection on CCTV feeds by combining YOLO and a Vision-Language Model (VLM) to achieve highly accurate filtering and labeling.

Detection: Ultralytics YOLO models (people_model, gun_model), fused for speed.
Tracking: supervision.ByteTrack per stream; side‑by‑side output for two feeds.
Re‑ID (prototype): ResNet50 embedding head (Identity() final layer) + cosine similarity to link cam2 IDs to cam1.(you can add deepsort for more accurate tracking)
Weapons heuristic: keyword filter and a dedicated YOLO weapon model.
Moondream VLM: per‑crop Q&A to enrich labels/attributes (e.g., “is anyone holding a gun?”).ios.

# read design thoughts for cooments and imporvement and here is a video explantion for it https://drive.google.com/file/d/1bOoc4_OO_SBYE7103tQfTFIVASeynmr1/view?usp=sharing

# Steps to run on colab:

Just run the New notebook file on colab, runnng one cell after other, uploadt best.pt model, also your video for testing  or use the sample video shared

You will need moondream key, get it from here https://moondream.ai/ and add it to colab secrets

download results and to view them.






