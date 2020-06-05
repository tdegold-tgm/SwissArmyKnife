# TODO-App mit C#/Entity Framework Core

Tim Degold, 4AHIT, begonnen am 23.02.2020

## Installation von Entity Framework

Um EF verwenden zu können muss es installiert werden. Dazu in VisualStudio unter `Extras>NuGet-Paket-Manager>Paket-Manager-Konsole` die NuGet-Konsole öffnen und folgenden Befehl eingeben.

```shell
PM> install-package entityframework
```

Alle benötigten Abhängigkeiten werden installiert.

## App.config konfigurieren

Damit das Programm weiß, auf welche Datenbank es zugreifen muss, bzw. welche Datenbank erstellt werden muss, muss ein sog. Connection-String in der *App.config*-Datei angegeben werden. Wenn man mysql verwendet sieht er folgendermaßen aus.

```shell
<connectionStrings>
      <add name="<ContextClassName>" connectionString="server=<server ip/localhost>;
      user=<username>;database=<DBName>;password=<insy>;"
      providerName="System.Data.SqlClient"/>
</connectionStrings>
```

## Migrationen aktivieren und erstellen

Um nun Migrationen zu ermöglichen in der NuGet-Konsole

```
PM>Enable-Migrations
```

tippen. Dies sollte reibungslos funktionieren, wenn der Connection-String richtig gesetzt wurde.

Mit 

```
PM>add-migration <migrationname>
```

kannst du eine Migration erstellen und mit

```
PM>update-database
```

in die DB einspielen.

## Quellen 

[1] https://dotnetplaybook.com/introduction-to-entity-framework/

[2] https://dev.mysql.com/doc/connector-net/en/connector-net-entityframework60.html

[3] https://help.syncfusion.com/extension/syncfusion-nuget-packages/nuget-uninstallation-process

[4] https://stackoverflow.com/questions/24496960/ef6-codefirst-mysql-migrations-type-nvarcharmax-not-supported

[5] https://www.youtube.com/playlist?list=PLpSmZmoBaROYOxp50yy_uewyMr5rOmx1f