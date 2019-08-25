# packer-images
A collection of Hashicorp Packer images for various Cloud Platforms (mostly related automation, containers, and Kubernetes)

## Notice

I've decided to change the format for how the packer images in this repo are executed. Instead of having a collection of specific folders per packer artifact (which seemed incredibly wasteful and redundant), I'm forcing `BASH` environment variables to drive each of the installs. This way, the only thing that needs to be added are semi-intelligent scripts tied to a shell variable. When that variable is then called, either manually through a shell session or through a CI/CD system like Jenkins, only the things required are installed. Consideration must be given when ordering the installs, but this will simplify the overall repository greatly.

***NOTE:*** *these changes will occur over the course of the next few days.*

## Contributions

Please consider contributing rather than forking for the purpose of "saving" this repository. All contributions will be considered and reviewed. CI/CD coming soon! I'm just trying to decide if I should use [GitHub Actions](https://github.com/features/actions) or a project-level Jenkinsfile.
