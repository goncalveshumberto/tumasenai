# tumasenai
class cadastro{
    constructor(pNome, pEndereco, pBairro, pCep, pCidade, pEstado, pNascimento){
        this.nome = pNome;
        this.endereco = pEndereco;
        this.bairro = pBairro;
        this.cep = pCep;
        this.cidade = pCidade;
        this.estado = pEstado;
        this.nascimento = pNascimento;
    }
    Get nome(){
        return this.nome
    }
    set nome (pnome){
        this.nome = pNome;
    }
    Get endereco(){
        return this.endereco;
    }
    Set endereco(pEndereco){
        this.endereco = pEndereco;
    }
    Get bairro(){
        return this.bairro;
    }
    Set bairro(pBairro){
        this.bairro = pBairro;
    }
    Get cep(){
        return this.cep;
    }
    Set cep(pCep){
        this.cep = pCep;
    }
    get cidade(){
        return this.cidade;
    }
    set cidade(pCidade){
        this.cidade = pCidade;
    }
    get estado(){
        return this.estado;
    }
    set estado(pEstado){
        this.estado = pEstado;
    }
    get nascimento(){
        return this.nascimento;
    }
    set nascimento(pNascimento){
        this.nascimento = pNascimento;
    }
    imprimir(){
        return "Nome: " + this.nome +
            "\Endereço: " + this.endereco +
            "n\Bairro: " + this.bairro +
            "n\Cep: " + this.cep +
            "n\Cidade: " + this.cidade +
            "n\Estado: " + this.estado +
            "n\Data de Nascimento: " + this.nascimento;
    }
}

Class pessoafisica extends cadastro{
    constructor(pNome, pEndereco, pBairro, pCep, pCidade, pEstado, pNascimento, pCpf)
    super(pNome, pEndereco, pBairro, pCep, pCidade, pEstado, pNascimento);
    this.cpf = pCpf;
    get cpf(){
        return this.cpf;
    }
    set cpf(pCpf){
        this.cpf = pCpf;
    }
    imprimir(){
        return super.imprimir() + "\nCPF: " this.cpf;
    }
    }
Class pessoajuridica extends cadastro
    constructor(pNome, pEndereco, pBairro, pCep, pCidade, pEstado, pNascimento,pCnpj)
    super(pNome, pEndereco, pBairro, pCep, pCidade, pEstado, pNascimento);
    this.cnpj =pCnpj
    Get cnpj(){
        return this.cnpj;
    }
    Set cnpj(pCnpj){
        this.cnpj = pCnpj;
    }
    Imprimir (){
        return super.imprimir() + "n\CNPJ: " + this.cnpj;
    }
