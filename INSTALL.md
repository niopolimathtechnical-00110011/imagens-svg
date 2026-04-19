# 📦 Instalação - Ícones Matrix Mantra

## 📋 Pré-requisitos
- Sistema operacional Linux com GNOME
- Permissão de escrita no diretório de destino

## 🚀 Método 1: Instalação Local (Usuário atual)
```bash
git clone [https://github.com/nio00110011/imagens-svg.git](https://github.com/nio00110011/imagens-svg.git)
cd imagens-svg
cp -r icons/matrix-digital-rain-em-sanscrito-1.1 ~/.local/share/icons/

# O pacote estará disponível imediatamente

🖥️ Método 2: Instalação global (para todos os usuários)
bash

# Clone o repositório (ou baixe os arquivos)
git clone https://github.com/nio00110011/imagens-svg.git
cd imagens-svg

# Copie com privilégios de administrador
sudo cp -r icons/matrix-digital-rain-em-sanscrito-1.1 /usr/share/icons/

🎨 Método 3: Instalação manual (substituir ícones individuais)

Se você quiser substituir apenas ícones específicos:
bash

# Exemplo: substituir o ícone da pasta Documentos
cp icons/matrix-digital-rain-em-sanscrito-1.1/scalable/places/folder-documents.svg \
   ~/.local/share/icons/Adwaita/scalable/places/folder-documents.svg

# Ou para substituir diretamente no sistema (requer sudo)
sudo cp icons/matrix-digital-rain-em-sanscrito-1.1/scalable/places/folder-documents.svg \
        /usr/share/icons/Adwaita/scalable/places/folder-documents.svg

🔧 Ativando o tema no GNOME
Opção 1: GNOME Tweaks (interface gráfica)

    Instale o GNOME Tweaks:
    bash

    sudo apt install gnome-tweaks        # Debian/Ubuntu
    sudo pacman -S gnome-tweaks          # Arch/CachyOS
    sudo dnf install gnome-tweaks        # Fedora

    Abra o GNOME Tweaks

    Vá para Aparência → Ícones

    Selecione matrix-digital-rain-em-sanscrito-1.1

Opção 2: Linha de comando (gsettings)
bash

# Definir como tema de ícones atual
gsettings set org.gnome.desktop.interface icon-theme 'matrix-digital-rain-em-sanscrito-1.1'

# Voltar ao tema padrão Adwaita
gsettings set org.gnome.desktop.interface icon-theme 'Adwaita'

Opção 3: Substituição direta (sem ativar como tema)
bash

# Backup do ícone original
sudo cp /usr/share/icons/Adwaita/scalable/places/folder-documents.svg \
        /usr/share/icons/Adwaita/scalable/places/folder-documents.svg.bak

# Substituir pelo novo ícone
sudo cp icons/matrix-digital-rain-em-sanscrito-1.1/scalable/places/folder-documents.svg \
        /usr/share/icons/Adwaita/scalable/places/folder-documents.svg

📁 Mapeamento dos ícones
Ícone do pack /	Destino no sistema
folder-apps.svg	places/folder-apps.svg
folder-desktop.svg	places/user-desktop.svg
folder-documents.svg	places/folder-documents.svg
folder-download.svg	places/folder-download.svg
folder-music.svg	places/folder-music.svg
folder-network-workgroup.svg	places/network-workgroup.svg
folder-pictures.svg	places/folder-pictures.svg
folder-publicshare.svg	places/folder-publicshare.svg
folder-templates.svg	places/folder-templates.svg
folder-user-bookmarks.svg	places/user-bookmarks.svg
folder-user-home.svg	places/user-home.svg
folder-user-trash.svg	places/user-trash.svg
folder-videos.svg	places/folder-videos.svg


🔄 Desinstalação
Remover tema de ícones


# Remover do diretório do usuário
rm -rf ~/.local/share/icons/matrix-digital-rain-em-sanscrito-1.1

# Remover do sistema (requer sudo)
sudo rm -rf /usr/share/icons/matrix-digital-rain-em-sanscrito-1.1

# Voltar ao tema padrão
gsettings set org.gnome.desktop.interface icon-theme 'Adwaita'

Restaurar ícones individuais

# Restaurar backup
sudo mv /usr/share/icons/Adwaita/scalable/places/folder-documents.svg.bak \
        /usr/share/icons/Adwaita/scalable/places/folder-documents.svg

🐛 Solução de problemas
Problema: Os ícones não aparecem após a instalação

Solução: Reinicie o GNOME Shell (Alt+F2 → r → Enter) ou faça logout e login novamente.
Problema: Permissão negada

Solução: Use sudo para instalação global ou instale no diretório do usuário (~/.local/share/icons/).
Problema: O tema não aparece no GNOME Tweaks

Solução: Certifique-se de que a estrutura está correta:

ls ~/.local/share/icons/matrix-digital-rain-em-sanscrito-1.1/scalable/places/
# Deve mostrar todos os arquivos .svg

📞 Suporte

    GitHub Issues: @nio00110011

    Email: niopolimathtechnical@gmail.com

☕ Apoie o projeto com um café via PIX: soletrepix@gmail.com
