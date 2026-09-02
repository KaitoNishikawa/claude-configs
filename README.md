# Claude Configs

Shared Claude Code configuration and usage notes.

## Tips

### Give vision work tools to crop and zoom

Claude Fable 5.1 has better vision capabilities out of the box, and on complex visual inputs such as dense charts it does its best work when it can iteratively analyze, crop, and visually verify what it sees. To get the full benefit, run the model as an agent with access to a container that holds the raw images or videos and has basic image-processing libraries (such as PIL and OpenCV) pre-installed. If running a container is too much overhead, an image-cropping tool alone delivers most of the uplift: a tool that returns a chosen region of the image, cropped and enlarged, lets the model examine specific details in more depth and scales test-time compute with image tokens. The [crop tool recipe](https://platform.claude.com/cookbook/multimodal-crop-tool) has a working definition.
