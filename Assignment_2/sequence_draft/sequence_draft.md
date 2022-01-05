```mermaid
sequenceDiagram
    autonumber

    loop try login for 5 times

        student ->>+ dashbaordView: login(username, password) 
        dashbaordView ->>+ dashbaordController: login(username, password)
        dashbaordController ->>+ serverController: get_userinfo_object(username, password)
        serverController ->>+ userInfoPool: get_userinfo_boject(username, password) 
        userInfoPool ->>+ database: query_authenticate_user(username, password)


        database -->>- userInfoPool: userinfo_object
        userInfoPool -->>- serverController: userinfo_object
        serverController -->>- dashbaordController: userinfo_object
        dashbaordController -->>- dashbaordView: render_homepage(data)
        dashbaordView -->>- student: html, css, javascript

    end




```

    



