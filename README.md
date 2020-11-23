package Sitema;

import java.io.IOException;
import java.sql.SQLException;
import java.util.List;


import Categoria.Inicio;
import Materialconstrucao.Processo.ProcessamentoFerramenta;
import Materialconstrucao.Processo.ProcessamentoMaterial;
import Materialconstrucao.Registro.Registro;

public class Programa {
	public static void main(String[] args) throws IOException, SQLException {
		
		List<Registro> MenuMaterial = ProcessamentoMaterial.lerArquivoM("C:\\_ws\\construcao\\Material.txt");
	
List<Registro> MenuFerramenta = ProcessamentoFerramenta.lerArquivoF("C:\\_ws\\construcao\\Ferramentas.txt");
Inicio.Menu(MenuMaterial, MenuFerramenta);
}
}
