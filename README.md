# produtoscadastrados01
*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package valoresdosprodutos;

import java.util.ArrayList;
import java.util.List;

/**
 *
 * @author anali
 */
public class produtoscontroller {
   List<CadastroProduto> produtos = new ArrayList<>();

public void adicionar(CadastroProduto cp) {
    produtos.add(cp);
}

public void listaProdutos() {
    produtos.forEach((p) -> {
        System.out.println("Nome: " + p.getNome());
        System.out.println("Modelo: " + p.getModelo());
        System.out.println("Tamanho: " + p.getTamanho());
        System.out.println("Preço: " + p.getPreco());
        System.out.println("-----------------------------");
    });
} 

    public produtoscontroller() {
    }

    public List<CadastroProduto> getProdutos() {
        return produtos;
    }

    public void setProdutos(List<CadastroProduto> produtos) {
        this.produtos = produtos;
    }

    private static class CadastroProduto {

        public CadastroProduto() {
        }

        private String getNome() {
            throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
        }

        private String getModelo() {
            throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
        }

        private String getTamanho() {
            throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
        }

        private String getPreco() {
            throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
        }
    }
}
