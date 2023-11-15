#include <iostream>
#include <string>
#include <vector>

using namespace std;

struct Solicitacao {
  string nome;
  string cnpj;
  string tipo;
  string area;
  string local;
};

struct Avaliacao {
  bool aprovada;
  string motivo;
};

struct Licenca {
  string numero;
  string validade;
};

class EcoAutoriza {
public:
  EcoAutoriza() {}

  void cadastrarSolicitacao(Solicitacao solicitacao) {
    cout << "Solicitação cadastrada com sucesso!" << endl;
  }

  Avaliacao avaliarSolicitacao(Solicitacao solicitacao) {
    Avaliacao avaliacao;

    // Avaliar a solicitação de corte de árvore em área urbana
    if (solicitacao.tipo == "Corte de árvore" && solicitacao.local == "Área Urbana") {
      avaliacao.aprovada = true;
      avaliacao.motivo = "Solicitação de corte de árvore em área urbana aprovada";
    } else {
      avaliacao.aprovada = false;
      avaliacao.motivo = "Solicitação reprovada";
    }

    return avaliacao;
  }

  void aprovarSolicitacao(Solicitacao solicitacao, Avaliacao avaliacao) {
    cout << "Solicitação aprovada!" << endl;
  }

  void reprovarSolicitacao(Solicitacao solicitacao, Avaliacao avaliacao) {
    cout << "Solicitação reprovada!" << endl;
  }

  void verificarDocumentos(Solicitacao solicitacao) {
    // Verificar se todos os documentos necessários estão anexados à solicitação
    cout << "Documentos verificados com sucesso!" << endl;
  }

  void atribuirSolicitacao(Solicitacao solicitacao) {
    // Atribuir a solicitação a um técnico florestal (simulação)
    cout << "Solicitação atribuída ao técnico João Silva com sucesso!" << endl;
  }

  void comunicarSolicitante(Solicitacao solicitacao, Avaliacao avaliacao) {
    // Enviar um e-mail ao solicitante informando o status da solicitação
    string status = avaliacao.aprovada ? "Aprovada" : "Reprovada";
    cout << "Caro(a) " << solicitacao.nome << ", sua solicitação foi " << status << ". Motivo: " << avaliacao.motivo << endl;
  }

  void gerenciarSolicitacoes() {
    // Listar todas as solicitações cadastradas (simulação)
    cout << "Listagem de todas as solicitações:" << endl;
    // Implemente a lógica real de listagem aqui

    // Filtrar solicitações por status (simulação)
    cout << "Filtrar solicitações por status (Aprovadas):" << endl;
    // Implemente a lógica real de filtragem aqui

    // Pesquisar solicitações por nome, CNPJ ou tipo (simulação)
    cout << "Pesquisar solicitações por nome, CNPJ ou tipo (Pesquisa por nome 'Empresa A'):" << endl;
    // Implemente a lógica real de pesquisa aqui
  }

  void gerarAutorizacao(Solicitacao solicitacao, Avaliacao avaliacao) {
    // Gerar uma autorização com base na solicitação e na avaliação (simulação)
    cout << "Autorização gerada com sucesso para a solicitação de " << solicitacao.tipo << endl;
  }

  void registrarAutorizacao(Solicitacao solicitacao, Avaliacao avaliacao) {
    // Registrar a autorização no sistema (simulação)
    cout << "Autorização registrada com sucesso!" << endl;
  }

  void acompanharSolicitacao(Solicitacao solicitacao) {
    // Consultar o status da solicitação (simulação)
    cout << "Status da solicitação de " << solicitacao.nome << ": Em análise" << endl;

    // Visualizar os documentos anexados à solicitação (simulação)
    cout << "Documentos anexados à solicitação:" << endl;
    // Implemente a lógica real de visualização de documentos aqui
  }

  void comunicarTecnico(Solicitacao solicitacao) {
    // Enviar um e-mail ao técnico responsável pela solicitação (simulação)
    cout << "E-mail enviado ao técnico responsável informando sobre a nova solicitação." << endl;
  }

  void registrarLicenca(Solicitacao solicitacao, Avaliacao avaliacao) {
    // Gerar uma licença com base na solicitação e na avaliação (simulação)
    Licenca licenca;
    licenca.numero = "123456";
    licenca.validade = "2023-12-31";

    // Registrar a licença no sistema (simulação)
    cout << "Licença registrada com sucesso para a solicitação de " << solicitacao.tipo << endl;
  }
};

int main() {
  EcoAutoriza ecoAutoriza;

  Solicitacao solicitacao;
  solicitacao.nome = "Empresa A";
  solicitacao.cnpj = "12345678901234";
  solicitacao.tipo = "Corte de árvore";
  solicitacao.area = "10 hectares"; // Área de exemplo para corte de árvore
  solicitacao.local = "Área Urbana"; // Local alterado para "Área Urbana"

  ecoAutoriza.cadastrarSolicitacao(solicitacao);

  Avaliacao avaliacao = ecoAutoriza.avaliarSolicitacao(solicitacao);

  if (avaliacao.aprovada) {
    ecoAutoriza.verificarDocumentos(solicitacao);
    ecoAutoriza.atribuirSolicitacao(solicitacao);
    ecoAutoriza.comunicarSolicitante(solicitacao, avaliacao);
    ecoAutoriza.gerarAutorizacao(solicitacao, avaliacao);
    ecoAutoriza.registrarAutorizacao(solicitacao, avaliacao);
    ecoAutoriza.acompanharSolicitacao(solicitacao);
    ecoAutoriza.comunicarTecnico(solicitacao);
    ecoAutoriza.registrarLicenca(solicitacao, avaliacao);
  } else {
    ecoAutoriza.reprovarSolicitacao(solicitacao, avaliacao);
  }

  ecoAutoriza.gerenciarSolicitacoes(); // Chamando a função para gerenciar solicitações (simulação)

  return 0;
}
