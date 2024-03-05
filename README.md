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
http://email.redmineup.com/c/eJyEz81q6zAQhuGrkXcnSBqNfhZeHAje9RqMLI0SUUs2ilz38ksglG5Kty8Pw3xxTOgsLAONwnCnhUVjhvuIkLgwCpXRCrQNQTuNnhYC53mybsijRtIL2uSiWvgso0UyIjljFeCimOKNYsmVjv3fI3e6FJ_XYR3vve8M_jM5MTmd53n5ZpewFSanNQeqD5qLr_5GjclJaC4NZzD17Z0qgyt3FrURGBWEpDGYwA0KCjxJkFJ5ExRYJvXRy_zYjhaIwfXN5_pqhWI-CoMrPZ96xeDL7vPteT9uZ103H-d9PW65zj9Zp1b-IGGrnWr_TQ1tXOkze6Z49R_Unru_AgAA__8JWX9q

- 설치방법: https://www.redmineup.com/pages/help/agile/installing-redmine-agile-plugin-on-bitnami-stack?utm_source=Main&utm_medium=email&utm_campaign=Download_plugin_email&utm_term=download_plugin_email&utm_content=installation_guide
