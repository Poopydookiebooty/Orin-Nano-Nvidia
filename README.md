# Orin-Nano-Nvidia
how to code and train orin nano to detect food
#setting up
https://drive.google.com/file/d/1O6Tf47tW1rouejb4w4qwqZ2lK1J27-Nq/view

I used Visual studio code to make this code you must create a remote network and connect to the hotspot that you connected the nano.
add food datasets with Curl then train it with some codes(search it up) then open it up with https://github.com/dusty-nv/jetson-inference/blob/master/docs/webrtc-server.md -link net=~/ and then detectnet \
  --model=$NET/ssd-mobilenet.onnx \
  --labels=$NET/labels.txt \
  --input-blob=input_0 \
  --output-cvg=scores \
  --output-bbox=boxes \
  /dev/video0

open this up in a browser

Check out dusty's readme's for more info and help on your nanos.
