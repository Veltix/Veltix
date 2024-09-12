```php
<?php

namespace Veltix;

use Gained\KnowledgeBase\{ Php, Javascript, Css, Linux, Mysql, Lemp, 
                          Lamp, Laravel, Vuejs, DigitalOcean, Wordpress, 
                          Woocommerce, React, Tailwindcss, RestApi };

Class About extends Me
{
    public function __construct()
    {
        $this->github = 'Veltix';
        $this->age = 27;
        $this->location = 'Europe\Tallinn';
        $this->languages = ['PHP', 'Javascript', 'CSS'];
        $this->frameworks = ['Laravel', 'Vuejs', 'React', 'Tailwindcss'];
        $this->databases = ['Mysql'];
        $this->webStacks = ['LEMP', 'LAMP'];
        $this->cloudProviders = ['DigitalOcean', 'Hetzner'];
        $this->cms = ['Wordpress', 'Woocommerce'];
        $this->integrations = ['REST API', 'XML', 'JSON'];
    }

    protected function getWorkplace(): array
    {
        return [
            'company' => 'Web Design Agency OÜ',
            'position' => 'Full Stack Developer',
            'location' => 'Tallinn, Estonia'
        ];
    }

    public function getKnowledge(): array
    {
        return [
            Php::class,
            Javascript::class,
            Css::class,
            Linux::class,
            Mysql::class,
            Lemp::class,
            Lamp::class,
            Laravel::class,
            Vuejs::class,
            DigitalOcean::class,
            Wordpress::class,
            Woocommerce::class,
            React::class,
            Tailwindcss::class,
            RestApi::class
        ];
    }

    public function getHobbies(): array
    {
        return [
            'Coding',
            'Playing with my daughter',
            'Reading Documentations',
            'Traveling',
            'Learning',
            'Driving BMW',
            'Gym',
        ];
    }

    public function getQuote(): string
    {
        return 'Code is like humor. When you have to explain it, it’s bad. – Cory House';
    }


}
```