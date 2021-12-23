### Fix Flatpak Theme

Uma das inconveniências dos aplicativos empacotados como flatpaks é a possibilidade dos mesmos não identificarem os temas. Para solucionar basta copiar o arquivo `settings.ini` para a pasta de configuração do aplicativo flatpak.

### Settings.ini

`settings.ini` é o arquivo que guarda as informações de quais temas gtk você está usando. Exemplo:

```

[Settings]
gtk-theme-name=Arc-Dark
gtk-icon-theme-name=Papirus-Dark
gtk-font-name=Sans 10
gtk-cursor-theme-name=capitaine-cursors
gtk-cursor-theme-size=0
gtk-toolbar-style=GTK_TOOLBAR_BOTH
gtk-toolbar-icon-size=GTK_ICON_SIZE_LARGE_TOOLBAR
gtk-button-images=1
gtk-menu-images=1
gtk-enable-event-sounds=1
gtk-enable-input-feedback-sounds=1
gtk-xft-antialias=1
gtk-xft-hinting=1
gtk-xft-hintstyle=hintfull

```

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

![Image_01](https://i.imgur.com/WUuLcxc.png)

#### Blanket

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/com.rafaelmardojai.Blanket/config/gtk-3.0/"

```

![Image_02](https://i.imgur.com/8q7mwty.png)

#### Warpinator

```

cp -R $HOME/.config/gtk-3.0/settings.ini "$HOME/.var/app/org.x.Warpinator/config/gtk-3.0/"

```

![Image_03](https://i.imgur.com/JsPl0rM.png)

### Observações

Infelizmente alguns aplicativos podem não reconhecer algum tema. Sinceramente é frustante mas não sei o que pode ser. No meu caso, firefox e anki não reconheceu o cursor theme e cockatrice o arc theme.

### Contato

Caso tenha dúvidas sobre algo ou sugestões.

- Discord: JohnJohn1809#4864
- Telegram: @JohnJohn1809
