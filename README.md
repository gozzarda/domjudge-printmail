# domjudge-printmail
A mod to replace DOMJudge printing with emailing

- `docker exec -it domjudge-domserver bash`
- `cd /opt/domjudge/domserver/`
- Download PHPMailer
  - `cd /usr/share/php`
  - `apt update && apt install git`
  - `git clone https://github.com/PHPMailer/PHPMailer.git`
  - `cd -`
- Add `./webapp/src/DOMJudgeBundle/Utils/PrintMail.php`
- Replace `./webapp/src/DOMJudgeBundle/Controller/Team/MiscController.php`
