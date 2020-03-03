# Installing MCM App

## Steps

1. Download this project from git

2. Change the below values according to your cluster in the file `/src/mutual-subscription/21-placement.yaml` 

```
  clusterLabels:
    matchExpressions:
      - key: cloud
        operator: In
        values:
        - IBM
```

3. Goto `install` folder in command prompt

4. Set kubetcl context in commmand prompt that points to your mcm hub.

5. Run the below command.

```
sh 01-install.sh
```

The application get installed in the mcm hub.

6. Access your application with your browser using the url

```
http://<<IP_ADDRESS>>:31650
```