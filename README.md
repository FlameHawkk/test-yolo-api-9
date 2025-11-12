В файле "model_config.json" должно быть:

{
  "model_name": "yolov8n.pt",
  "translate_name": "coco.csv",
  "font_file": "Geoform.ttf"
}

или

{
  "model_name": "yolov8n-oiv7.pt",
  "translate_name": "OpenImagesV7.csv",
  "font_file": "Geoform.ttf"
}

или

{
  "model_name": "yolo11n.pt",
  "translate_name": "coco.csv",
  "font_file": "Geoform.ttf"
}

или для другой по аналогии.

Важно: Шрифт нужен с поддержкой кирилицы.

Render:
uvicorn main:app --host 0.0.0.0 --port $PORT