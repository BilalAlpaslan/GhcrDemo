# GhcrDemo
Github container registary demo


# to build

$ docker build -t ghcr.io/bilalalpaslan/ghcrdemo .

# to run

$ docker run -it --rm --name ghcrdemo ghcr.io/bilalalpaslan/ghcrdemo

# to push

$ docker push ghcr.io/bilalalpaslan/ghcrdemo

# of course you need to login to ghcr.io first with your github personal access token

$ echo $CR_PAT | docker login ghcr.io -u USERNAME --password-stdin

if this step be successfull, you can see the output like this: "Login Succeeded"

# to pull

$ docker pull ghcr.io/bilalalpaslan/ghcrdemo

# if you want push specific version of your image

$ docker tag ghcrdemo ghcr.io/bilalalpaslan/ghcrdemo:1.0.0