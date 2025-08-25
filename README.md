# Real-Time Object Detection with YOLO + VLM

This project demonstrates real-time object detection on CCTV feeds by combining YOLO and a Vision-Language Model (VLM) to achieve highly accurate filtering and labeling.

Overview

YOLO detects objects in video frames in real-time.

VLM refines YOLO’s predictions, generating a JSONL dataset with more accurate labels for each frame.

The JSONL output can be used to fine-tune YOLO models, improving detection accuracy on specific scenarios or environments.

Workflow

Real-Time Detection – YOLO processes CCTV feeds, identifying objects and generating initial frame annotations.

VLM Refinement – The VLM analyzes the detected frames, correcting mislabels and adding contextual details.

Dataset Generation – The VLM outputs JSONL files mapping frames to refined labels.

YOLO Fine-Tuning – Use the JSONL dataset to retrain YOLO for improved performance on the target data.

Benefits

Improved Accuracy: VLM helps correct errors and adds context YOLO may miss.

Real-Time Performance: YOLO handles fast processing while VLM adds minimal overhead.

Custom Dataset Creation: Easily generate high-quality labeled datasets for specialized scenarios.
