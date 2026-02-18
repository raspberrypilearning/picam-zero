
The best Python library for controlling the Raspberry Pi Camera Module is `picamzero`. To get started, check out [this project guide](https://raspberrypifoundation.github.io/picamzero/hello_world/){:target="_blank"} for a handy walkthrough of how to install and use it.


#### Usage

```python
from picamzero import Camera
from time import sleep

camera = Camera()

# Take a picture every minute for 3 hours
for i in range(3*60):
    camera.take_photo(f'image_{i:03d}.jpg')
    sleep(60)
```

#### Documentation

- [https://raspberrypifoundation.github.io/picamzero](https://raspberrypifoundation.github.io/picamzero){:target="_blank"}
