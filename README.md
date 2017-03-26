# exception-monitor

Why this project ?
------------------
I'm working for a web agency that needs to monitor more than 50 websites.

We are using a custom solution, because using a SaaS solution would be too expensive.

Furthermore, our intern solution is developer oriented and project owners doesn't know what is really happening.

This project goal is to create an application that will be focused on project owners' use.

Key features
------------
- Catch exception
- Assigns an error to an user
- Tags an exception
- Track deployment
  - There's a deploy hook addon for heroku 
  - `heroku addons:create deployhooks:http --url=http://service.com`
- Add exception to a service
  - Gitlab
  - Trello
  - webhook
- Snooze error notification for a certain amount of time

Existing Solutions
-----------------
- https://sentry.io
- https://www.honeybadger.io
- https://airbrake.io (you need a credit card to test it... urgh...)
- https://rollbar.com
- https://raygun.com

Sentry unique features
---------
- Custom alert
![sentry-01-alert-setting.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-01-alert-setting.png?raw=true)
![sentry-02-alerts.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-02-alerts.png?raw=true)
![sentry-03-add-alert.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-03-add-alert.png?raw=true)
![sentry-04-new-rule.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-04-new-rule.png?raw=true)
![sentry-05-new-rule-condition.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-05-new-rule-condition.png?raw=true)
![sentry-06-new-rule-trigger.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-06-new-rule-trigger.png?raw=true)
![sentry-07-new-rule-action.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-07-new-rule-action.png?raw=true)
- Custom search filter
![sentry-08-custom-search-filter.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-08-custom-search-filter.png?raw=true)
- User feedback on error
![sentry-09-user-feedback.png](https://github.com/nicolas-besnard/exception-monitor/blob/master/images/sentry-09-user-feedback.png?raw=true)
