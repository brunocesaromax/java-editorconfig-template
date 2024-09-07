# Java EditorConfig Template

Este repositório contém um arquivo `.editorconfig` padrão para projetos Java, projetado para manter a consistência de estilo de código entre diferentes editores e IDEs.

## O que é EditorConfig?

EditorConfig ajuda a manter estilos de codificação consistentes para múltiplos desenvolvedores trabalhando no mesmo projeto em diferentes editores e IDEs. O EditorConfig consiste em um formato de arquivo para definir estilos de codificação e uma coleção de plugins de editor de texto que permitem aos editores ler o formato de arquivo e aderir aos estilos definidos.

## Como usar

1. Clone este repositório ou baixe o arquivo `.editorconfig`.
2. Copie o arquivo `.editorconfig` para a raiz do seu projeto Java.
3. Se seu editor não suportar EditorConfig nativamente, instale o plugin apropriado (veja [editorconfig.org](https://editorconfig.org) para uma lista de plugins).

## Configurações

Nosso arquivo `.editorconfig` inclui as seguintes configurações:

```editorconfig
# EditorConfig para projetos Java
# https://editorconfig.org/

# Configuração de nível superior para todos os arquivos
root = true

[*]
charset = utf-8
end_of_line = lf
indent_style = space
indent_size = 4
insert_final_newline = true
trim_trailing_whitespace = true

# Configurações específicas para arquivos Java
[*.java]
max_line_length = 120

# Configurações para arquivos XML (comuns em projetos Java)
[*.xml]
indent_size = 2

# Configurações para arquivos de propriedades
[*.properties]
charset = latin1

# Configurações para arquivos Markdown
[*.md]
trim_trailing_whitespace = false

# Configurações para arquivos YAML (como configurações do Maven ou Gradle)
[*.{yml,yaml}]
indent_size = 2

# Configurações para arquivos de script shell
[*.sh]
end_of_line = lf

# Configurações para arquivos batch do Windows
[*.bat]
end_of_line = crlf
```

### Detalhes das configurações

- **charset**: UTF-8 para a maioria dos arquivos, Latin1 para arquivos `.properties`.
- **end_of_line**: LF (Line Feed) para a maioria dos arquivos, CRLF para arquivos batch do Windows.
- **indent_style**: Espaços para todos os arquivos.
- **indent_size**: 4 espaços para a maioria dos arquivos, 2 para XML e YAML.
- **insert_final_newline**: Garante que o arquivo termine com uma nova linha.
- **trim_trailing_whitespace**: Remove espaços em branco no final das linhas (exceto para arquivos Markdown).
- **max_line_length**: 120 caracteres para arquivos Java.

## Contribuindo

Sinta-se à vontade para propor mudanças abrindo uma issue ou enviando um pull request. Toda contribuição é bem-vinda!

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

## Recursos adicionais

- [EditorConfig](https://editorconfig.org/)
- [Java Code Conventions](https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)
- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
