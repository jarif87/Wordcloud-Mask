# Read Image From Online

```import requests```

```from PIL import Image```

```from io import BytesIO```

```import matplotlib.pyplot as plt```


```url = "https://raw.githubusercontent.com/jarif87/wordcloud-png/main/batman.png"```


```response = requests.get(url)```

```image_content = response.content```


```image = Image.open(BytesIO(image_content))```

```plt.figure(figsize=(10,10))```

```plt.imshow(image)```

```plt.show()```
