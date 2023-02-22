
Build Docker Image
```
$docker build --build-arg GIT_ACCESS_TOKEN=[insert-access-token-here] -t [image_name]:[image_tag] .
```
More specifically:
```
$docker build --build-arg GIT_ACCESS_TOKEN=[insert-access-token-here] -t rpack-atlas:v2.12.0 .
```

Run Docker Container
```
$docker run --name rpack-atlas -e USER=user -e PASSWORD=password -p 8787:8787 rpack-atlas:v2.12.0
```