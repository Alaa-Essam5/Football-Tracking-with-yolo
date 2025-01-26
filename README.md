# Football Player Tracking with YOLO

This project demonstrates how to use a pretrained YOLO (You Only Look Once) AI model to track players in a football game. It allows users to select a player, and then displays a heatmap showing their movement throughout the game. The heatmap visualizes the areas where the player has spent most of their time, giving insights into their movement patterns.

## Features

- **Player Detection**: Using the YOLO model, players are detected in real-time from video footage of a football game.
- **Player Selection**: Users can select a player they want to track.
- **Movement Heatmap**: A heatmap is generated showing the player's movement throughout the game, indicating areas of high and low activity.
  
## Requirements

To run this project, you will need:

- Python 3.x
- OpenCV (for video processing)
- NumPy (for handling array operations)
- TensorFlow or PyTorch (depending on which framework YOLO is implemented in)
- Pretrained YOLOv4 or YOLOv5 model weights
- Matplotlib (for displaying the heatmap)
  
You can install the necessary dependencies with the following command:

```bash
pip install opencv-python numpy tensorflow matplotlib
```

For YOLO, follow the installation steps in the [YOLO repository](https://github.com/AlexeyAB/darknet) or use a PyTorch implementation like [YOLOv5](https://github.com/ultralytics/yolov5).

## Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/football-player-tracking.git
    cd football-player-tracking
    ```

2. Download the pretrained YOLO model weights. You can download YOLOv4 weights from the [YOLO website](https://pjreddie.com/darknet/yolo/), or use YOLOv5 weights from the [YOLOv5 GitHub](https://github.com/ultralytics/yolov5).

3. Place the model weights file in the `models/` directory.

## Usage

1. **Detect Players**: Once the video is loaded, the pretrained YOLO model will automatically detect and track players in the video.
2. **Select Player**: Click on a detected player to select them for tracking.
3. **Generate Heatmap**: After selecting the player, a heatmap of their movement will be displayed in real-time, showing areas of high activity in red and lower activity in blue.

To run the program, use the following command:

```bash
python tracking.py --video your_video_file.mp4
```

Replace `your_video_file.mp4` with the path to the football game video you want to process.

## Code Structure

- `tracking.py`: Main script that runs the player detection and tracking.
- `yolo_model.py`: YOLO model implementation and loading of the pretrained weights.
- `finalheatmap.py`: Code to generate and display the heatmap.
- `gui.py`: Graphical user interface (GUI) for player selection and video visualization.
- `trackingtry.py`: Experimental script for additional tracking functionalities or tests.

## Example Output

After running the script, you should see something like this:

- A window with the video where players are detected and labeled.
- After selecting a player, a heatmap will appear showing their movement pattern.

# 🌟 Watch the Demo Video Here! 🌟
https://github.com/user-attachments/assets/d3b9862f-f2b7-4a8a-aff7-1959675bcdab

## Contributing

If you'd like to contribute to this project, feel free to fork the repository, submit issues, or create pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Let me know if you'd like further modifications!
