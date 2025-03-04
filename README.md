sudo apt-get install git-flow

gerando chave assinatura
pull request 
default branch develop
block signature
block commit in main

#branch and commit
git checkout develop
git checkout -b feature/name
git add .
git commit -m 'commit name'


#Semantic Versioning 2.0.0
https://semver.org/
Given a version number MAJOR.MINOR.PATCH, increment the:

MAJOR version when you make incompatible API changes
MINOR version when you add functionality in a backward compatible manner
PATCH version when you make backward compatible bug fixes
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.


#Conventional Commits:
https://www.conventionalcommits.org/pt-br/v1.0.0/#especifica%c3%a7%c3%a3o
https://github.com/conventional-commits/conventionalcommits.org

<tipo>[escopo opcional]: <descrição>
BREAKING CHANGE: <descrição> podem ser providos e seguem uma convenção similar ao git
build:, chore:, ci:, docs:, style:, refactor:, perf:, test:
fix: e feat:

[corpo opcional]

[rodapé(s) opcional(is)]
feat: permitir que o objeto de configuração fornecido estenda outras configurações
BREAKING CHANGE: a chave `extends`, no arquivo de configuração, agora é utilizada para estender outro arquivo de configuração



#Ferramenta para garantir que seus commits estejam em conformidade com commits convencionais . Ela é voltada principalmente para CIs para evitar branches com commits que não estejam em conformidade. O uso como um hook de pré-commit também está sob consideração.
https://commitsar.aevea.ee/usage/docker/
docker run --rm --name="commitsar" -w /src -v "$(pwd)":/src aevea/commitsar 
docker run --rm --name="commitsar" -w /src -v "$(pwd)":/src aevea/commitsar ./path-to-repo