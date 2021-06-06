
# Hardhat-Dockerized

<script type="text/javascript"
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.3/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

Run [Hardhat](https://hardhat.org/) in a Docker Container 

Follow the Instructions at [README](https://github.com/NicolaBernini/Hardhat-Dockerized/)



# Instructions 

## 1. Build the image 

Run 

```
build.sh
```

This will create the `my_hardhat:v0.1` docker image in your local registry 





## 2. Run a container 

Go to your project dir and run 

```
run.sh
```

NOTE 

- Of course you have to make sure `run.sh` is in your path or you have to use the absolute path pointing at this file 

This will mount `PWD` into the `/project` directory in the container 



## 3. Start a Project 

Run 

```
npx hardhat test
```

If the `/project` directory is empty, that command will start and interactive CLI to define the project parameters and at the end of this process the scaffolding of a test project will be created 



Running again 

```
npx hardhat test
```

with this scaffolding will compile the project and run the tests 




