```php
$developer = new Dev(
    name:  'ThinhNQ',
    email: 'thinhnq@vn.ids.jp',
    age:   33
);

$developer->setStatus(new Life\Status(
    learning:   ['PHP', 'Reactjs', 'Software Architecture'],
    exploring:  ['AWS'],
    aiming:     ['']
));

$mySkills = new Life\Skills(
    languages:   ['PHP', 'Bash', 'HTML/CSS', 'JavaScript', 'PowerShell'],
    editors:     ['PHPStorm', 'VS Code', 'Notepad++', 'Vim'],
    frameworks:  ['Bootstrap', 'Laravel', 'jQuery'],
    databases:   ['PostgreSQL', 'MySQL', 'Redis', 'MongoDB'],
    techStack:   [
        'Git', 'Gitlab CI/CD', 'Markdown', 'Postman',
        'Docker', 'Docker Compose', 'RabbitMQ', 'WebSocket',
        'Vagrant', 'WSL2', 'Zsh', 'Nginx', 'PHP-FPM', 'Jekyll',
        'Memcached', 'MailHog', 'CentOS', 'Ubuntu'
    ]
);

$developerRole = new Career\Developer(person: $developer, skills: $mySkills);

while ($developerRole->hasCoffee())  
{
    $developerRole->code();
}

```