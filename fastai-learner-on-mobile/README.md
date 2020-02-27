## serving a fast.ai learner via mobile web browser :) #edgedeployment

> if you like living on the edge

> **What's going on:**  
> start a web app off of this notebook with [Voila](https://github.com/voila-dashboards/voila)  
> tunnel your local server to the world with [ngrok](https://ngrok.com/)  
> navigate to your website from your smartphone  
> tap the big upload button, take a photo, get predictions


this notebook loads an MNIST learner (with a black-on-white transform).

Adapt it to work for your own model!


## launching

> you'll need a learner - modify the notebook to load an existing learner that you have trained

```sh
voila --port 7878 widgit.ipynb
```

then, in a separate terminal:  

```sh
ngrok http [--region=eu] 7878
```

Go to the ngrok URL on your phone and upload photos! :)