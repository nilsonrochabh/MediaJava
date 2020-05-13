package media;

import javax.swing.JOptionPane;

import classes.Aluno;

public class ClasseMedia {
	public static void main(String[] args) {
		
		//ainda não existe
		Aluno aluno1;
		
		//agora existe
		Aluno aluno2=new Aluno();
		
		String nota1=JOptionPane.showInputDialog("Informe a primeira nota");
		String nota2=JOptionPane.showInputDialog("Informe a segunda nota");
		String nota3=JOptionPane.showInputDialog("Informe a terceira nota");
		String nota4=JOptionPane.showInputDialog("Informe a quarta nota");
		
		double dNota1=Double.parseDouble(nota1);
		double dNota2=Double.parseDouble(nota2);
		double dNota3=Double.parseDouble(nota3);
		double dNota4=Double.parseDouble(nota4);
		
		double mediaFinal = (dNota1 + dNota2 + dNota3 + dNota4) / 4;
		
		if (mediaFinal >= 50) {
			if(mediaFinal>=70) {
				JOptionPane.showMessageDialog(null, "Aluno(a) aprovado com a média : "+mediaFinal);
			}else {
				JOptionPane.showMessageDialog(null, "Aluno(a) em recuperação com a média : "+mediaFinal);
			}
			
			
		}
		else {
			JOptionPane.showMessageDialog(null, "Aluno(a) Reprovado com a média : "+mediaFinal);
		}
	}
}
