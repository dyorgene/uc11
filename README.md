# Nome do Projeto

Leilões TDS - UC11

## Explicação do Projeto

Atividade 1 da UC11, praticar versionamento local e remoto, fazer em Java utilizar banco de dados

## Tecnologias Utilizadas

- Java
- MySQL

## Exemplo de Código

```java

public class conectaDAO {
    
    public Connection connectDB(){
        Connection conn = null;
        
        try {
        
            conn = DriverManager.getConnection("jdbc:mysql://localhost/uc11?user=root&password=");
            
        } catch (SQLException erro){
            JOptionPane.showMessageDialog(null, "Erro ConectaDAO" + erro.getMessage());
        }
        return conn;
    }
    
}

```
