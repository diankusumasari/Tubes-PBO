# Tubes-PBO
// Customizable //
public interface Costumizable{
	public void setBGColor();
	public void setFont();
}
// Jadwal //
import java.util.Date;
public class Jadwal{
	private Date jam;
	private Date tanggal;
	private Date hari;
	public Jadwal(Date jam, Date tanggal, Date hari){
		this.jam = jam;
		this.tanggal = tanggal;
		this.hari = hari;
	}
	public Date getJam(){
		return jam;
	}
	public Date getHari(){
		return hari;
	}
	public Date getTanggal(){
		return tanggal;
	}
	public String toString(){
		return "Blablabla";
	}
}
// Task //
public class Task implements Customizable{
	private Jadwal jadwal;
	private String jenis, status, deskripsi, judul;
	public void setStatus(){
		this.status = "Belum";
	}
	
}
