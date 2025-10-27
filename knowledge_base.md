Important Questions

1. Why the size of docker image is less?
A: Layer Reuse:
Docker reuses common layers across images, so only unique parts add size.

Minimal Base Images:
Images like alpine or scratch start very small (as low as a few MB).

Multi-Stage Builds:
Unnecessary build tools are excluded from the final image — only the app remains.

Compression:
Images are compressed when stored or pushed, making them appear smaller.

Shared Layers at Runtime:
Containers share read-only image layers, reducing disk usage.