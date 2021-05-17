---
title: "Galvanorte Galvanização - Serviços de Galvanização a Fogo"
head-title: "Galvanização a Fogo"
description: "A galvanização a fogo (zincagem a quente) é uma forma econômica de proteger vigas, tubos, cantoneiras, chapas, estruturas e peças contra a corrosão."
featured: true
weight: 5
layout: service
---

Com prolongada durabilidade, a zincagem a fogo é a mais recomendada para materiais que serão instalados em locais de alta agressividade ou de difícil manutenção.

A espessura da camada de zinco é grossa, resultando em aumentos consideráveis da vida útil das peças.

Estamos em fase de análise e projeto para **iniciar no futuro** a prestação de serviço de galvanização a fogo, atendendo o Paraná e sul de São Paulo. Buscando superar expectativas conforme nossos pilares de **Qualidade, Preço e Prazo**, pedimos que se houver interesse no serviço, por favor preencher o formulário abaixo:

<script type='text/javascript' src='//code.jquery.com/jquery-compat-git.js'></script>
<script type='text/javascript' src='//igorescobar.github.io/jQuery-Mask-Plugin/js/jquery.mask.min.js'></script>

<link rel="stylesheet" href="/assets/css/skeleton.css">
<link rel="stylesheet" href="/assets/css/normalize.css">
<script>
    $(document).ready(function () {
        var behavior = function (val) {
            return val.replace(/\D/g, '').length === 11 ? '(00) 00000-0000' : '(00) 0000-00009';
        },
        options = {
            onKeyPress: function (val, e, field, options) {
                field.mask(behavior.apply({}, arguments), options);
            }
        };
        $('.phone').mask(behavior, options);
        $('form').submit(function( event ) {
            $('.button-primary').prop("disabled",true)
            datastring = $('form').serialize()
            $.ajax({
                type: "POST",
                url: "https://script.google.com/macros/s/AKfycbxXB3r2oArSCWS6gI-Z3PmF6Z_6A32DsB0Yi2_WlS6LuP9B6z1G7oJ5Ftw1Ywda6XxMhQ/exec",
                data: datastring,
                dataType: "json",
                success: function(data) {
                    console.log(data)     
                    $('.button-primary').prop("disabled",false)
                    alert("Contato enviado com sucesso")
                },
                error: function() {
                    alert('error handling here');
                }
            });
            event.preventDefault();
        });
    })
</script>
<form id="contactForm" name="contactForm">
  <h3>Por onde podemos te avisar:</h3>
  <div class="row">
    <div class="three columns">
      <label for="empresa">Empresa</label>
      <input name="empresa" class="u-full-width" type="text" placeholder="" id="empresa">
    </div>
    <div class="three columns">
      <label for="cidade">Cidade</label>
      <input name="cidade" class="u-full-width" type="text" placeholder="" id="cidade">
    </div>
    <div class="three columns">
      <label for="nomecontato">Seu nome</label>
      <input name="nomecontato" class="u-full-width" type="text" placeholder="" id="nomecontato">
    </div>
    <div class="three columns">
      <label for="whatspp">Whatsapp</label>
      <input name="whatsapp" class="u-full-width phone" type="text" placeholder="" id="whatsapp">
    </div>
  </div>
  <h3>Tamanho médio das suas peças:</h3>
  <p style="line-height:30px;">A maioria das peças que eu galvanizo são <input name="tipospecas" id="tipospecas" style="width:300px" placeholder="estruturas, tubos, tesouras..." />, e na média as maiores chegam a ter aprox. <input name="tamanhospecas" id="tamanhospecas" placeholder="comp. x altura x largura" /> em metros. Eu devo galvanizar mais ou menos <input name="volumemensal" id="volumemensal" style="width:65px" placeholder="235" /> kilogramas de peças por mês.</p>
  <div>
    <a href="https://api.whatsapp.com/send?phone=5543999143694&text=Ol%C3%A1.%20Tenho%20algumas%20pe%C3%A7as%20para%20galvanizar%20a%20fogo.">
        <button type="button">
        <img src="https://www.convertte.com.br/cvtt/wp-content/themes/cvtt_v3/assets/gerador-link-new/images/wpp-logo.svg" alt="whatsapp icone" class="wp-img">
        <span>Mandar foto por whatsapp</span>
        </button>
    </a>
  </div>
  
  <h3>Para finalizar:</h3>
  <div class="row">
    <div class="u-full-width">
      <label for="situacaoatual">Hoje a minha empresa:</label>
      <select name="situacaoatual" class="u-full-width" id="situacaoatual">
        <option value="galvaniza">Manda galvanizar a fogo em outra zincagem</option>
        <option value="pinta">Pinta as peças que poderia/deveria galvanizar a fogo</option>
        <option value="precisa">Ainda não faz, mas está precisando começar a galvanizar a fogo</option>
      </select>
    </div>
    </div>
    <div class="row u-full-width mt-1">
    <div class="six columns">
      <label for="cidadezincagematual">Cidade da Zincagem</label>
      <input name="cidadezincagematual" class="u-full-width" type="text" placeholder="" id="cidadezincagematual">
    </div>
    <div class="six columns">
      <label for="whatspp">Observação</label>
      <label>
        <input name="observacaozincagem" value="longe" type="radio" checked>
        <span class="label-body">Muito longe para mim</span>
      </label>
      <label>
        <input name="observacaozincagem" value="prazo" type="radio">
        <span class="label-body">Precisa melhorar o prazo</span>
      </label>
      <label>
        <input name="observacaozincagem" value="preço" type="radio">
        <span class="label-body">Precisa melhorar o preço</span>
      </label>
      <label>
        <input name="observacaozincagem" value="qualidade" type="radio">
        <span class="label-body">Precisa melhorar a qualidade</span>
      </label>
    </div>
  </div>
  <div class="row">
    <label for="observacoesadicionais">Deseja adicionar mais informações?</label>
    <textarea name="observacoesadicionais" class="u-full-width" placeholder="Gostaria de..." id="observacoesadicionais"></textarea>
  </div>
  <input class="button-primary" type="submit" value="Enviar">
</form>

<style>
    form .row {
        margin-bottom:20px;
    }
    .wp-img {
        height: 20px !important;
        margin: auto !important;
    }
</style>