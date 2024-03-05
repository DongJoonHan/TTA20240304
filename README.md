# TTA20240304
Redmine 교육

# Redmine 다운로드
(https://www.dropbox.com/scl/fi/yj7almkm7jzghi43mue28/bitnami-redmine-4.2.4-0-windows-x64-installer.exe?rlkey=itr3hf1p76uulnr2wza9802yg&dl=0)https://www.dropbox.com/scl/fi/yj7almkm7jzghi43mue28/bitnami-redmine-4.2.4-0-windows-x64-installer.exe?rlkey=itr3hf1p76uulnr2wza9802yg&dl=0

# Redmine Home 위치
```sh
C:\Bitnami\redmine-4.2.4-0\apps\redmine\htdocs
```

이동 방법
- 우선, bitnami package의 CMD를 실행한 후, 다음 명령 입력
```sh
cd apps\redmine\htdocs
```

# Plugin
## Issue Template
- 홈페이지 위치: https://github.com/agileware-jp/redmine_issue_templates
- 설치 명령
```sh
bundle exec rails redmine:plugins:migrate RAILS_ENV=production
```
- 명령 실행 후 Redmine 재시작

## Agile 

- 설치방법: https://www.redmineup.com/pages/help/agile/installing-redmine-agile-plugin-on-bitnami-stack?utm_source=Main&utm_medium=email&utm_campaign=Download_plugin_email&utm_term=download_plugin_email&utm_content=installation_guide

# Redmine API 사용 예
```sh
curl "http://RedmineURL/redmine/issues.json" -X POST --header "Content-Type: application/json" --header "X-Redmine-API-Key: 6c597ababa6fcc69147fba626647c9280c4ecf15" --data-binary "@../redmine_AP.json"
```

# Redmine 백업 복원 참조
https://kmin135.blogspot.com/2017/08/bitnami-redmine.html

# Checksum 확인
```sh
certutil -hashfile "파일명" SHA256|MD5
```
예
```sh
certuil -hashfile junit.jar SHA256
```
