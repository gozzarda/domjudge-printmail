# domjudge-printmail
A mod to replacing DOMJudge printing with emailing

- `docker exec -it domjudge-domserver bash`
- `cd /opt/domjudge/domserver/`
- Download PHPMailer
  - `cd lib`
  - `apt update && apt install git`
  - `git clone https://github.com/PHPMailer/PHPMailer.git`
  - `cd ..`
- Add `./webapp/src/DOMJudgeBundle/Utils/PrintMail.php`
- Replace `./webapp/src/DOMJudgeBundle/Controller/Team/MiscController.php`
