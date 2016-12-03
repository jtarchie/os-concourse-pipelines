# OSS Projects Concourse Pipelines

As an experiment, I've been trying to convert `.travis.yml` to their equivalent concourse pipelines. These pipelines use ERB for templating as the DSL from `.travis.yml` doesn't map 1-to-1.

## Usage

To sync a pipeline with concourse.ci deployment:

```
fly set-pipeline -p nokogiri -c <(erb pipelines/nokogiri.yml)
```
