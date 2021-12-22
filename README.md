### Fix Flatpak Theme

Uma das inconveniências dos aplicativos empacotados como flatpaks é a possibilidade dos mesmos não identificarem os temas. Para solucionar basta copiar o arquivo `settings.ini` para a pasta de configuração do aplicativo flatpak.

### Fixing

Copie o arquivo `settings.ini` para a pasta de configuração do aplicativo flatpak. O arquivo `settings.ini` fica no caminho `$HOME/.config/gtk-3.0/`. Exemplo:

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/path.to.you.flatpak/config/gtk-3.0/"

```

### Exemple with Real Paths

#### Drawing

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/com.github.maoschanz.drawing/config/gtk-3.0/"

```

#### Blanket

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/com.rafaelmardojai.Blanket/config/gtk-3.0/"

```

#### Warpinator

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/org.x.Warpinator/config/gtk-3.0/"

```
