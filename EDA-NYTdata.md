



<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled is-u2f-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-cb4ede7df6d8670c4051172e4d6bc6916b3c765fa15b4ee9b348f157fdb85114.css" integrity="sha256-y07effbYZwxAURcuTWvGkWs8dl+hW07ps0jxV/24URQ=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-171d3f0f3e5bd93fdd10a9f389e058c1f415ee10ec550302a2b73c5aaf70ce2e.css" integrity="sha256-Fx0/Dz5b2T/dEKnzieBYwfQV7hDsVQMCorc8Wq9wzi4=" media="all" rel="stylesheet" />
    
    
    
    

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    <title>stat6306introdatascience/EDA-NYTdata.md at master · MonnieMcGee/stat6306introdatascience</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars0.githubusercontent.com/u/14001220?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="MonnieMcGee/stat6306introdatascience" name="twitter:title" /><meta content="stat6306introdatascience - Files and projects for Stat 6306 Introduction to Data Science" name="twitter:description" />
      <meta content="https://avatars0.githubusercontent.com/u/14001220?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="MonnieMcGee/stat6306introdatascience" property="og:title" /><meta content="https://github.com/MonnieMcGee/stat6306introdatascience" property="og:url" /><meta content="stat6306introdatascience - Files and projects for Stat 6306 Introduction to Data Science" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/MjI2NjczMjg6YmZkY2Q2MWViOGNlYTA4YWVjNDQ2OGFiYjgxZmU3OWQ6N2FhNjA3OWE3OGEzZWNkZjAyNmI0MjQ1MmMzNmVjZDEwNDg5MTFjZDUyNTFmMDA1MjA0YWYyNDJmNWVhYzU1MQ==--9c8a363061a07bcb5eb3f9db076383e0fc72508d">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">
    <meta name="request-id" content="4C64503B:0E04:3961AEB:57FBEC8B" data-pjax-transient>

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="4C64503B:0E04:3961AEB:57FBEC8B" name="octolytics-dimension-request_id" /><meta content="22667328" name="octolytics-actor-id" /><meta content="mnaples81" name="octolytics-actor-login" /><meta content="e831d57157b521b09615c3ff98436822cd1a2730c280ec727fa57f0a4c110981" name="octolytics-actor-hash" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged In">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="mnaples81">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="Y2MyMzlmNGI4NTc4MzYyMjJiMWY1NDZhM2ZmN2QxMzg5NDcxMzQ5NjhjZjljZjYzOTRjYmViMjAxM2NhN2ZkMHx7InJlbW90ZV9hZGRyZXNzIjoiNzYuMTAwLjgwLjU5IiwicmVxdWVzdF9pZCI6IjRDNjQ1MDNCOjBFMDQ6Mzk2MUFFQjo1N0ZCRUM4QiIsInRpbWVzdGFtcCI6MTQ3NjEyNzg4NH0=">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="1b94697933c5b8a5a903245bdfd54f28787b35f6">
    <meta content="dbda80d4725e1fe34426a1e02f300e7698e66b26" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="f83d92fe4867e9c2c4edb7b8588f3f24">
    

      
  <meta name="description" content="stat6306introdatascience - Files and projects for Stat 6306 Introduction to Data Science">
  <meta name="go-import" content="github.com/MonnieMcGee/stat6306introdatascience git https://github.com/MonnieMcGee/stat6306introdatascience.git">

  <meta content="14001220" name="octolytics-dimension-user_id" /><meta content="MonnieMcGee" name="octolytics-dimension-user_login" /><meta content="41495288" name="octolytics-dimension-repository_id" /><meta content="MonnieMcGee/stat6306introdatascience" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="41495288" name="octolytics-dimension-repository_network_root_id" /><meta content="MonnieMcGee/stat6306introdatascience" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/MonnieMcGee/stat6306introdatascience/commits/master.atom" rel="alternate" title="Recent Commits to stat6306introdatascience:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata.md" data-pjax-transient>
  </head>


  <body class="logged-in  env-production windows vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg aria-hidden="true" class="octicon octicon-mark-github" height="28" version="1.1" viewBox="0 0 16 16" width="28"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>


        <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/search" class="js-site-search-form" data-scoped-search-url="/MonnieMcGee/stat6306introdatascience/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
    </label>
</form></div>


      <ul class="header-nav float-left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" aria-label="Pull requests you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" aria-label="Issues you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav float-right" id="user-links">
  <li class="header-nav-item">
    

  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <svg aria-hidden="true" class="octicon octicon-plus float-left" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 9H7v5H5V9H0V7h5V2h2v5h5z"></path></svg>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>


  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="MonnieMcGee/stat6306introdatascience">This repository</span>
  </div>
    <a class="dropdown-item" href="/MonnieMcGee/stat6306introdatascience/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-sw js-menu-target" href="/mnaples81"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@mnaples81" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/22667328?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu dropdown-menu-sw">
        <div class="dropdown-header header-nav-current-user css-truncate">
          Signed in as <strong class="css-truncate-target">mnaples81</strong>
        </div>

        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/mnaples81" data-ga-click="Header, go to profile, text:your profile">
          Your profile
        </a>
        <a class="dropdown-item" href="/mnaples81?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
        <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
          Explore
        </a>
          <a class="dropdown-item" href="/integrations" data-ga-click="Header, go to integrations, text:integrations">
            Integrations
          </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>


        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
          Settings
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="oIqCvl0SGHFYMF/9lmO/8wlenCYxczKZYiFYMHOWfa7Gk+9kVDWHPpCSWAZMDQY6yfRLPmA0x85Tv4LUbgNIhg==" /></div>
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>


      


    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="Fi4D7A11KOA4t7OPep2G79UJztNfbEejCwSzgMuDueA028G0QJ7+sLaCGG8MJn/CQgGF9mlKcl3fOjHtX4tCZQ==" /></div>      <input class="form-control" id="repository_id" name="repository_id" type="hidden" value="41495288" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/MonnieMcGee/stat6306introdatascience/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
              <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
              Watch
            </span>
          </a>
          <a class="social-count js-social-count"
            href="/MonnieMcGee/stat6306introdatascience/watchers"
            aria-label="1 user is watching this repository">
            1
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_ignore" name="do" type="radio" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-mute" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"></path></svg>
                      Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/unstar" class="starred" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="Vz8+qfLAP6pbwn8osvXic7UDJ2KzjksUn1IEWz2fkzwxLMAut7GnDIQkak1G9XD2zSPwSEjqd6bifdMt5swDBw==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar MonnieMcGee/stat6306introdatascience"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/MonnieMcGee/stat6306introdatascience/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/star" class="unstarred" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="E18fdRSBmzWfP8usmikSYrLz3AErAflteGCUeJZDP7RF8zlKi+TpPgMfvOkVDg1KmoU2LCF7C/4K/P58jXqJ/w==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star MonnieMcGee/stat6306introdatascience"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/MonnieMcGee/stat6306introdatascience/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>  </div>

  </li>

  <li>
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/fork" class="btn-with-count" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="tjLu0OmMIG4LdnKNgMTm00YFEzmASkIoYUOz0S3Euc+K5v6IZgR3o2Er7UkyRGkxZgrfqPhVkyeMc3Y58/LWTw==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of MonnieMcGee/stat6306introdatascience to your account"
                aria-label="Fork your own copy of MonnieMcGee/stat6306introdatascience to your account">
              <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
              Fork
            </button>
</form>
    <a href="/MonnieMcGee/stat6306introdatascience/network" class="social-count"
       aria-label="64 users are forked this repository">
      64
    </a>
  </li>
</ul>

    <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"></path></svg>
  <span class="author" itemprop="author"><a href="/MonnieMcGee" class="url fn" rel="author">MonnieMcGee</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/MonnieMcGee/stat6306introdatascience" data-pjax="#js-repo-pjax-container">stat6306introdatascience</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/MonnieMcGee/stat6306introdatascience" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /MonnieMcGee/stat6306introdatascience" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"></path></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/MonnieMcGee/stat6306introdatascience/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /MonnieMcGee/stat6306introdatascience/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"></path></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/MonnieMcGee/stat6306introdatascience/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /MonnieMcGee/stat6306introdatascience/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">2</span>
      <meta itemprop="position" content="3">
</a>  </span>

  <a href="/MonnieMcGee/stat6306introdatascience/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /MonnieMcGee/stat6306introdatascience/projects">
    <svg class="octicon" aria-hidden="true" version="1.1" width="15" height="16" viewBox="0 0 15 16">
      <path d="M1 15h13V1H1v14zM15 1v14a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V1a1 1 0 0 1 1-1h13a1 1 0 0 1 1 1zm-4.41 11h1.82c.59 0 .59-.41.59-1V3c0-.59 0-1-.59-1h-1.82C10 2 10 2.41 10 3v8c0 .59 0 1 .59 1zm-4-2h1.82C9 10 9 9.59 9 9V3c0-.59 0-1-.59-1H6.59C6 2 6 2.41 6 3v6c0 .59 0 1 .59 1zM2 13V3c0-.59 0-1 .59-1h1.82C5 2 5 2.41 5 3v10c0 .59 0 1-.59 1H2.59C2 14 2 13.59 2 13z"></path>
    </svg>
    Projects
    <span class="counter">0</span>
</a>
    <a href="/MonnieMcGee/stat6306introdatascience/wiki" class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /MonnieMcGee/stat6306introdatascience/wiki">
      <svg aria-hidden="true" class="octicon octicon-book" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"></path></svg>
      Wiki
</a>

  <a href="/MonnieMcGee/stat6306introdatascience/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /MonnieMcGee/stat6306introdatascience/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"></path></svg>
    Pulse
</a>
  <a href="/MonnieMcGee/stat6306introdatascience/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /MonnieMcGee/stat6306introdatascience/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"></path></svg>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/MonnieMcGee/stat6306introdatascience/blob/70bb5e6f0a4dd1d7b26cb6811b4de125366c3c97/EDA-NYTdata.md" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:712bf095370b6135f42f6d8adec4135f -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="BtnGroup float-right">
    <a href="/MonnieMcGee/stat6306introdatascience/find/master"
          class="js-pjax-capture-input btn btn-sm BtnGroup-item"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/MonnieMcGee/stat6306introdatascience"><span>stat6306introdatascience</span></a></span></span><span class="separator">/</span><strong class="final-path">EDA-NYTdata.md</strong>
  </div>
</div>

<include-fragment class="commit-tease" src="/MonnieMcGee/stat6306introdatascience/contributors/master/EDA-NYTdata.md">
  <div>
    Fetching contributors&hellip;
  </div>

  <div class="commit-tease-contributors">
    <img alt="" class="loader-loading float-left" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" />
    <span class="loader-error">Cannot retrieve contributors at this time</span>
  </div>
</include-fragment>
<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata.md" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/MonnieMcGee/stat6306introdatascience/blame/master/EDA-NYTdata.md" class="btn btn-sm js-update-url-with-hash BtnGroup-item">Blame</a>
      <a href="/MonnieMcGee/stat6306introdatascience/commits/master/EDA-NYTdata.md" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="https://windows.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg aria-hidden="true" class="octicon octicon-device-desktop" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"></path></svg>
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/edit/master/EDA-NYTdata.md" class="inline-form js-update-url-with-hash" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="qO/5cBQPrZD+qnd/Ax8cDKpdhbw2AZVKnKHixZsh6uabkx8vn4q3xdnoKP9oRZO8kucqgsMXBA5MhrjOYPLdJQ==" /></div>
          <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and edit the file" data-hotkey="e" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"></path></svg>
          </button>
</form>        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/MonnieMcGee/stat6306introdatascience/delete/master/EDA-NYTdata.md" class="inline-form" data-form-nonce="dbda80d4725e1fe34426a1e02f300e7698e66b26" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="0zZ4vmU0tVyDb5JCct1vQ7L2cP/smBdHHA8gpafFeLhH+Dq/CTk9mzfFWHXL5R3bsWfbnJnsax1NfOsypcciyQ==" /></div>
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and delete the file" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"></path></svg>
          </button>
</form>  </div>

  <div class="file-info">
      376 lines (305 sloc)
      <span class="file-info-divider"></span>
    12 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-eda-nytclicks" class="anchor" href="#eda-nytclicks" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>EDA-NYTClicks</h1>

<p>Monnie McGee<br>
September 9, 2015  </p>

<p>This is the R markdown document for keeping track of code used to explore the NYT clicks data from May 1, 2012. </p>

<p>Required packages: doBy and ggplot2. Install and/or load these packages before trying the code below.</p>

<div class="highlight highlight-source-r"><pre>library(<span class="pl-smi">ggplot2</span>)
library(<span class="pl-smi">doBy</span>)</pre></div>

<pre><code>## Loading required package: survival
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Enter the data</span>
<span class="pl-smi">fileLocation</span> <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>http://stat.columbia.edu/~rachel/datasets/nyt1.csv<span class="pl-pds">"</span></span>
<span class="pl-smi">data1</span> <span class="pl-k">&lt;-</span> read.csv(url(<span class="pl-smi">fileLocation</span>))
names(<span class="pl-smi">data1</span>) <span class="pl-c"># What are the variable names?</span></pre></div>

<pre><code>## [1] "Age"         "Gender"      "Impressions" "Clicks"      "Signed_In"
</code></pre>

<div class="highlight highlight-source-r"><pre>str(<span class="pl-smi">data1</span>)</pre></div>

<pre><code>## 'data.frame':    458441 obs. of  5 variables:
##  $ Age        : int  36 73 30 49 47 47 0 46 16 52 ...
##  $ Gender     : int  0 1 0 1 1 0 0 0 0 0 ...
##  $ Impressions: int  3 3 3 3 11 11 7 5 3 4 ...
##  $ Clicks     : int  0 0 0 0 0 1 1 0 0 0 ...
##  $ Signed_In  : int  1 1 1 1 1 1 0 1 1 1 ...
</code></pre>

<p>The "str" function (pronounced "stir") tells us that all of the variables are in integer format. We may want to change the format of certain variables later, depending on what we are doing with the variable.</p>

<h2><a id="user-content-task-1-exploratory-data-analysis" class="anchor" href="#task-1-exploratory-data-analysis" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Task 1: Exploratory Data Analysis</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Numerical summary of the data. A good place to start. </span>
summary(<span class="pl-smi">data1</span>)</pre></div>

<pre><code>##       Age             Gender       Impressions         Clicks       
##  Min.   :  0.00   Min.   :0.000   Min.   : 0.000   Min.   :0.00000  
##  1st Qu.:  0.00   1st Qu.:0.000   1st Qu.: 3.000   1st Qu.:0.00000  
##  Median : 31.00   Median :0.000   Median : 5.000   Median :0.00000  
##  Mean   : 29.48   Mean   :0.367   Mean   : 5.007   Mean   :0.09259  
##  3rd Qu.: 48.00   3rd Qu.:1.000   3rd Qu.: 6.000   3rd Qu.:0.00000  
##  Max.   :108.00   Max.   :1.000   Max.   :20.000   Max.   :4.00000  
##    Signed_In     
##  Min.   :0.0000  
##  1st Qu.:0.0000  
##  Median :1.0000  
##  Mean   :0.7009  
##  3rd Qu.:1.0000  
##  Max.   :1.0000
</code></pre>

<h2><a id="user-content-question-signed_in-and-gender-are-both-indicator-variables-what-does-the-mean-of-each-of-these-variables-tell-us" class="anchor" href="#question-signed_in-and-gender-are-both-indicator-variables-what-does-the-mean-of-each-of-these-variables-tell-us" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> Signed_In and Gender are both indicator variables. What does the mean of each of these variables tell us?</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># distribution of ages</span>
hist(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Age</span>, <span class="pl-v">main</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-v">xlab</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>Age<span class="pl-pds">"</span></span>)</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-1.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-1.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre>quantile(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Age</span>) </pre></div>

<pre><code>##   0%  25%  50%  75% 100% 
##    0    0   31   48  108
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># distribution of Impressions</span>
hist(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span>, <span class="pl-v">main</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-v">xlab</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span># of Impressions<span class="pl-pds">"</span></span>)</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-2.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-2.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre>quantile(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span>)</pre></div>

<pre><code>##   0%  25%  50%  75% 100% 
##    0    3    5    6   20
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># distribution of Clicks</span>
hist(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Clicks</span>, <span class="pl-v">main</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-v">xlab</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span># of Clicks<span class="pl-pds">"</span></span>)</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-3.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-4-3.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre>quantile(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Clicks</span>)</pre></div>

<pre><code>##   0%  25%  50%  75% 100% 
##    0    0    0    0    4
</code></pre>

<p>It looks like that Age is the only continuous variable. Clicks and Impressions are probably discrete (what makes me think that?). Let's use the 'table' function to determine the values of Clicks and Impressions and how many cases are assigned to each.</p>

<div class="highlight highlight-source-r"><pre>table(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Clicks</span>)</pre></div>

<pre><code>## 
##      0      1      2      3      4 
## 418603  37372   2330    127      9
</code></pre>

<div class="highlight highlight-source-r"><pre>table(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span>)</pre></div>

<pre><code>## 
##     0     1     2     3     4     5     6     7     8     9    10    11 
##  3066 15483 38433 64121 80303 80477 66808 48066 30081 16965  8357  3771 
##    12    13    14    15    16    17    18    20 
##  1549   647   211    64    25    11     2     1
</code></pre>

<h2><a id="user-content-question-what-do-we-learn-from-the-table-function" class="anchor" href="#question-what-do-we-learn-from-the-table-function" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> What do we learn from the table function?</h2>

<h2><a id="user-content-question-what-does-does-the-function-tabledata1agegroupdata1clicks-tell-us" class="anchor" href="#question-what-does-does-the-function-tabledata1agegroupdata1clicks-tell-us" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> What does does the function "table(data1$AgeGroup,data1$Clicks)" tell us?</h2>

<h2><a id="user-content-task-2-create-a-new-variable-for-age-groups-that-categorizes-users-as-18-18-24-25-34-35-44-45-54-55-64-and-65" class="anchor" href="#task-2-create-a-new-variable-for-age-groups-that-categorizes-users-as-18-18-24-25-34-35-44-45-54-55-64-and-65" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Task 2: Create a new variable for age groups that categorizes users as "&lt;18", "18-24", "25-34", "35-44", "45-54", "55-64", and "65+".</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Create age groups</span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">AgeGroup</span> <span class="pl-k">&lt;-</span> cut(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Age</span>, c(<span class="pl-k">-</span><span class="pl-c1">Inf</span>, <span class="pl-c1">18</span>, <span class="pl-c1">24</span>, <span class="pl-c1">34</span>, <span class="pl-c1">44</span>, <span class="pl-c1">54</span>, <span class="pl-c1">64</span>, <span class="pl-c1">Inf</span>))
levels(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">AgeGroup</span>) <span class="pl-k">&lt;-</span> c(<span class="pl-s"><span class="pl-pds">"</span>&lt;18<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>18-24<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>25-34<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>35-44<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>45-54<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>55-64<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>65+<span class="pl-pds">"</span></span>)
summaryBy(<span class="pl-smi">Gender</span><span class="pl-k">+</span><span class="pl-smi">Signed_In</span><span class="pl-k">+</span><span class="pl-smi">Impressions</span><span class="pl-k">+</span><span class="pl-smi">Clicks</span><span class="pl-k">~</span><span class="pl-smi">AgeGroup</span>, <span class="pl-v">data</span><span class="pl-k">=</span><span class="pl-smi">data1</span>)</pre></div>

<pre><code>##   AgeGroup Gender.mean Signed_In.mean Impressions.mean Clicks.mean
## 1      &lt;18  0.07906215      0.1231277         4.999571  0.14072193
## 2    18-24  0.53385313      1.0000000         5.006635  0.04845478
## 3    25-34  0.53216213      1.0000000         4.993829  0.05048647
## 4    35-44  0.53169630      1.0000000         5.021507  0.05167937
## 5    45-54  0.52897897      1.0000000         5.010406  0.05027377
## 6    55-64  0.53618848      1.0000000         5.022308  0.10183736
## 7      65+  0.36326644      1.0000000         5.012347  0.15128856
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Create a function. What does this function do?</span>
<span class="pl-en">siterange</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span>(<span class="pl-smi">x</span>){c(<span class="pl-v">n</span><span class="pl-k">=</span>length(<span class="pl-smi">x</span>),<span class="pl-v">MIN</span><span class="pl-k">=</span>min(<span class="pl-smi">x</span>),<span class="pl-v">MEAN</span><span class="pl-k">=</span>mean(<span class="pl-smi">x</span>),<span class="pl-v">MAX</span><span class="pl-k">=</span>max(<span class="pl-smi">x</span>))}
summaryBy(<span class="pl-smi">Age</span><span class="pl-k">~</span><span class="pl-smi">AgeGroup</span>, <span class="pl-v">data</span><span class="pl-k">=</span><span class="pl-smi">data1</span>, <span class="pl-v">FUN</span><span class="pl-k">=</span><span class="pl-smi">siterange</span>)</pre></div>

<pre><code>##   AgeGroup  Age.n Age.MIN  Age.MEAN Age.MAX
## 1      &lt;18 156358       0  1.974168      18
## 2    18-24  35270      19 21.269039      24
## 3    25-34  58174      25 29.503352      34
## 4    35-44  70860      35 39.494680      44
## 5    45-54  64288      45 49.492580      54
## 6    55-64  44738      55 59.498189      64
## 7      65+  28753      65 72.988697     108
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Histogram of Impressions by Age Group</span>
ggplot(<span class="pl-smi">data1</span>,aes(<span class="pl-v">x</span><span class="pl-k">=</span><span class="pl-smi">Impressions</span>,<span class="pl-v">fill</span><span class="pl-k">=</span><span class="pl-smi">AgeGroup</span>))<span class="pl-k">+</span>geom_histogram(<span class="pl-v">binwidth</span><span class="pl-k">=</span><span class="pl-c1">1</span>)</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-6-1.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-6-1.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Boxplot of Impressions by Age Group</span>
ggplot(<span class="pl-smi">data1</span>,aes(<span class="pl-v">x</span><span class="pl-k">=</span><span class="pl-smi">AgeGroup</span>,<span class="pl-v">y</span><span class="pl-k">=</span><span class="pl-smi">Impressions</span>))<span class="pl-k">+</span>geom_boxplot()</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-6-2.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-6-2.png" alt="" style="max-width:100%;"></a> </p>

<h2><a id="user-content-question-why-are-there-individuals-that-are-0-years-old-in-the-data-set-describe-these-individuals-using-the-other-variables-should-we-delete-these-individuals-from-the-data-set-why-or-why-not--the-code-below-is-a-good-starting-place-what-else-would-you-want-to-do-if-anything" class="anchor" href="#question-why-are-there-individuals-that-are-0-years-old-in-the-data-set-describe-these-individuals-using-the-other-variables-should-we-delete-these-individuals-from-the-data-set-why-or-why-not--the-code-below-is-a-good-starting-place-what-else-would-you-want-to-do-if-anything" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> Why are there individuals that are 0 years old in the data set? Describe these individuals using the other variables. Should we delete these individuals from the data set? Why or why not?  The code below is a good starting place. What else would you want to do (if anything)?</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-smi">dataChild</span> <span class="pl-k">&lt;-</span> subset(<span class="pl-smi">data1</span>, <span class="pl-smi">Age</span><span class="pl-k">==</span><span class="pl-c1">0</span>)
dim(<span class="pl-smi">dataChild</span>)</pre></div>

<pre><code>## [1] 137106      6
</code></pre>

<div class="highlight highlight-source-r"><pre>summary(<span class="pl-smi">dataChild</span>)</pre></div>

<pre><code>##       Age        Gender   Impressions     Clicks         Signed_In
##  Min.   :0   Min.   :0   Min.   : 0   Min.   :0.0000   Min.   :0  
##  1st Qu.:0   1st Qu.:0   1st Qu.: 3   1st Qu.:0.0000   1st Qu.:0  
##  Median :0   Median :0   Median : 5   Median :0.0000   Median :0  
##  Mean   :0   Mean   :0   Mean   : 5   Mean   :0.1421   Mean   :0  
##  3rd Qu.:0   3rd Qu.:0   3rd Qu.: 6   3rd Qu.:0.0000   3rd Qu.:0  
##  Max.   :0   Max.   :0   Max.   :18   Max.   :4.0000   Max.   :0  
##                                                                   
##   AgeGroup     
##  &lt;18  :137106  
##  18-24:     0  
##  25-34:     0  
##  35-44:     0  
##  45-54:     0  
##  55-64:     0  
##  65+  :     0
</code></pre>

<div class="highlight highlight-source-r"><pre>summaryBy(<span class="pl-smi">Signed_In</span><span class="pl-k">+</span><span class="pl-smi">Clicks</span><span class="pl-k">+</span><span class="pl-smi">Impressions</span><span class="pl-k">~</span><span class="pl-smi">Gender</span>,<span class="pl-v">data</span><span class="pl-k">=</span><span class="pl-smi">dataChild</span>,<span class="pl-v">FUN</span><span class="pl-k">=</span><span class="pl-smi">siterange</span>)</pre></div>

<pre><code>##   Gender Signed_In.n Signed_In.MIN Signed_In.MEAN Signed_In.MAX Clicks.n
## 1      0      137106             0              0             0   137106
##   Clicks.MIN Clicks.MEAN Clicks.MAX Impressions.n Impressions.MIN
## 1          0   0.1420799          4        137106               0
##   Impressions.MEAN Impressions.MAX
## 1         4.999657              18
</code></pre>

<h2><a id="user-content-question-does-gender0-always-mean-that-the-user-is-female-why-or-why-not" class="anchor" href="#question-does-gender0-always-mean-that-the-user-is-female-why-or-why-not" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> Does Gender=0 always mean that the user is female? Why or why not?</h2>

<h2><a id="user-content-task-3-for-a-single-day-plot-distributions-of-number-impressions-and-click-through-rate-ctr--clickimpressions-for-these-age-categories" class="anchor" href="#task-3-for-a-single-day-plot-distributions-of-number-impressions-and-click-through-rate-ctr--clickimpressions-for-these-age-categories" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Task 3: For a single day, plot distributions of number impressions and click-through-rate (CTR = click/impressions) for these age categories</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Define a new variable to segment Impressions into two groups</span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">hasImps</span> <span class="pl-k">&lt;-</span> cut(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span>, c(<span class="pl-k">-</span><span class="pl-c1">Inf</span>,<span class="pl-c1">0</span>,<span class="pl-c1">Inf</span>))
summaryBy(<span class="pl-smi">Clicks</span><span class="pl-k">~</span><span class="pl-smi">hasImps</span>, <span class="pl-v">data</span><span class="pl-k">=</span><span class="pl-smi">data1</span>, <span class="pl-v">FUN</span><span class="pl-k">=</span><span class="pl-smi">siterange</span>)</pre></div>

<pre><code>##    hasImps Clicks.n Clicks.MIN Clicks.MEAN Clicks.MAX
## 1 (-Inf,0]     3066          0  0.00000000          0
## 2 (0, Inf]   455375          0  0.09321768          4
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Create a factor based on Impressions and Clicks</span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">scode</span>[<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span> <span class="pl-k">==</span> <span class="pl-c1">0</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>NoImps<span class="pl-pds">"</span></span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">scode</span>[<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span> <span class="pl-k">&gt;</span> <span class="pl-c1">0</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>Imps<span class="pl-pds">"</span></span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">scode</span>[<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">Clicks</span> <span class="pl-k">&gt;</span> <span class="pl-c1">0</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>Clicks<span class="pl-pds">"</span></span>
<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">scode</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">data1</span><span class="pl-k">$</span><span class="pl-smi">scode</span>)
head(<span class="pl-smi">data1</span>)</pre></div>

<pre><code>##   Age Gender Impressions Clicks Signed_In AgeGroup  hasImps  scode
## 1  36      0           3      0         1    35-44 (0, Inf]   Imps
## 2  73      1           3      0         1      65+ (0, Inf]   Imps
## 3  30      0           3      0         1    25-34 (0, Inf]   Imps
## 4  49      1           3      0         1    45-54 (0, Inf]   Imps
## 5  47      1          11      0         1    45-54 (0, Inf]   Imps
## 6  47      0          11      1         1    45-54 (0, Inf] Clicks
</code></pre>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Create a function. What does it do?</span>
<span class="pl-en">clen</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span>(<span class="pl-smi">x</span>){c(length(<span class="pl-smi">x</span>))}
<span class="pl-smi">etable</span> <span class="pl-k">&lt;-</span> summaryBy(<span class="pl-smi">Impressions</span><span class="pl-k">~</span><span class="pl-smi">scode</span><span class="pl-k">+</span><span class="pl-smi">Gender</span><span class="pl-k">+</span><span class="pl-smi">AgeGroup</span>,<span class="pl-v">data</span><span class="pl-k">=</span><span class="pl-smi">data1</span>,<span class="pl-v">FUN</span><span class="pl-k">=</span><span class="pl-smi">clen</span>)
<span class="pl-smi">etable</span></pre></div>

<pre><code>##     scode Gender AgeGroup Impressions.clen
## 1  Clicks      0      &lt;18            18622
## 2  Clicks      0    18-24              779
## 3  Clicks      0    25-34             1361
## 4  Clicks      0    35-44             1675
## 5  Clicks      0    45-54             1494
## 6  Clicks      0    55-64             2006
## 7  Clicks      0      65+             2598
## 8  Clicks      1      &lt;18             1525
## 9  Clicks      1    18-24              890
## 10 Clicks      1    25-34             1509
## 11 Clicks      1    35-44             1917
## 12 Clicks      1    45-54             1645
## 13 Clicks      1    55-64             2331
## 14 Clicks      1      65+             1486
## 15   Imps      0      &lt;18           124402
## 16   Imps      0    18-24            15538
## 17   Imps      0    25-34            25690
## 18   Imps      0    35-44            31290
## 19   Imps      0    45-54            28563
## 20   Imps      0    55-64            18626
## 21   Imps      0      65+            15585
## 22   Imps      1      &lt;18            10754
## 23   Imps      1    18-24            17807
## 24   Imps      1    25-34            29241
## 25   Imps      1    35-44            35512
## 26   Imps      1    45-54            32143
## 27   Imps      1    55-64            21499
## 28   Imps      1      65+             8887
## 29 NoImps      0      &lt;18              972
## 30 NoImps      0    18-24              124
## 31 NoImps      0    25-34              165
## 32 NoImps      0    35-44              219
## 33 NoImps      0    45-54              224
## 34 NoImps      0    55-64              118
## 35 NoImps      0      65+              125
## 36 NoImps      1      &lt;18               83
## 37 NoImps      1    18-24              132
## 38 NoImps      1    25-34              208
## 39 NoImps      1    35-44              247
## 40 NoImps      1    45-54              219
## 41 NoImps      1    55-64              158
## 42 NoImps      1      65+               72
</code></pre>

<h2><a id="user-content-question-what-does-etable-tell-us" class="anchor" href="#question-what-does-etable-tell-us" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> What does 'etable' tell us?</h2>

<h2><a id="user-content-question-what-does-it-mean-to-have-zero-impressions-what-does-it-mean-to-have-zero-impressions-and-a-postive-number-of-clicks" class="anchor" href="#question-what-does-it-mean-to-have-zero-impressions-what-does-it-mean-to-have-zero-impressions-and-a-postive-number-of-clicks" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> What does it mean to have zero Impressions? What does it mean to have zero Impressions and a postive number of clicks?</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-c"># Create plot of CTR for a subset of the data where Impressions &gt; 0</span>
<span class="pl-smi">d1</span> <span class="pl-k">&lt;-</span> subset(<span class="pl-smi">data1</span>, <span class="pl-smi">Impressions</span> <span class="pl-k">&gt;</span> <span class="pl-c1">0</span>)
<span class="pl-smi">d1</span><span class="pl-k">$</span><span class="pl-smi">CTR</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">d1</span><span class="pl-k">$</span><span class="pl-smi">Clicks</span><span class="pl-k">/</span><span class="pl-smi">d1</span><span class="pl-k">$</span><span class="pl-smi">Impressions</span>
ggplot(<span class="pl-smi">d1</span>,aes(<span class="pl-v">x</span><span class="pl-k">=</span><span class="pl-smi">CTR</span>, <span class="pl-v">colour</span><span class="pl-k">=</span><span class="pl-smi">AgeGroup</span>))<span class="pl-k">+</span>geom_density()</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-1.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-1.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre>ggplot(subset(<span class="pl-smi">d1</span>, <span class="pl-smi">Clicks</span> <span class="pl-k">&gt;</span><span class="pl-c1">0</span>),aes(<span class="pl-v">x</span><span class="pl-k">=</span><span class="pl-smi">CTR</span>, <span class="pl-v">colour</span><span class="pl-k">=</span><span class="pl-smi">AgeGroup</span>))<span class="pl-k">+</span>geom_density()</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-2.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-2.png" alt="" style="max-width:100%;"></a> </p>

<div class="highlight highlight-source-r"><pre>ggplot(subset(<span class="pl-smi">d1</span>, <span class="pl-smi">CTR</span><span class="pl-k">&gt;</span><span class="pl-c1">0</span>), aes(<span class="pl-v">x</span><span class="pl-k">=</span><span class="pl-smi">CTR</span>, <span class="pl-v">fill</span><span class="pl-k">=</span><span class="pl-smi">AgeGroup</span>))<span class="pl-k">+</span>
    labs(<span class="pl-v">title</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>Click-through rate by age group (05/01/2012)<span class="pl-pds">"</span></span>)<span class="pl-k">+</span>
    geom_histogram(<span class="pl-v">binwidth</span><span class="pl-k">=</span>.<span class="pl-c1">025</span>)</pre></div>

<p><a href="/MonnieMcGee/stat6306introdatascience/blob/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-3.png" target="_blank"><img src="/MonnieMcGee/stat6306introdatascience/raw/master/EDA-NYTdata_files/figure-html/unnamed-chunk-9-3.png" alt="" style="max-width:100%;"></a> </p>

<h2><a id="user-content-question-summarize-these-plots-what-do-they-tell-you-about-the-relationship-between-click-through-rate-and-age" class="anchor" href="#question-summarize-these-plots-what-do-they-tell-you-about-the-relationship-between-click-through-rate-and-age" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><strong>Question:</strong> Summarize these plots. What do they tell you about the relationship between Click through rate and age?</h2>

<h2><a id="user-content-task-4" class="anchor" href="#task-4" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Task 4</h2>

<ul>
<li>Define a new variable to segment users based on their click behavior</li>
<li>Explore the data and make visual comparisons of click behavior across user segments</li>
<li>Create metrics/measurements/statistics that summarize the data
Note that this is an unordered list. You can do this in any order.</li>
</ul>

<h2><a id="user-content-case-study-i-due-october-1" class="anchor" href="#case-study-i-due-october-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Case Study I due October 1</h2>

<ul>
<li>Extend this analysis across days</li>
<li>Visualize some metrics and distributions over time</li>
<li>Describe and interpret any patterns you find</li>
<li>Put it all in an R markdown (or md) document
Note: This will take time. You will need to use Google and StackOverflow and other help. You will not be able to analyze absolutely everything. You have other classes. Pick one or two questions of interest to you (not to me!) and concentrate on those.</li>
</ul>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.16429s from github-fe-c5e6852.cp1-iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
      </button>
      You can't perform that action at this time.
    </div>


      
      <script crossorigin="anonymous" integrity="sha256-u8ByW3Q46gf3lKMTt8lghhPBANPkJ7NpsnoMo37E37w=" src="https://assets-cdn.github.com/assets/frameworks-bbc0725b7438ea07f794a313b7c9608613c100d3e427b369b27a0ca37ec4dfbc.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-b9yV+3zHS9yU513758mtwQYhu+wbOSi9ExWNJ+n48Rg=" src="https://assets-cdn.github.com/assets/github-6fdc95fb7cc74bdc94e75dfbe7c9adc10621bbec1b3928bd13158d27e9f8f118.js"></script>
      
      
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
    </button>
  </div>
</div>

  </body>
</html>

