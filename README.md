# Tubes-PBO
<br>// Customizable //</br>
<br>public interface Costumizable{</br>
        <br>public void setBGColor();</br>
        <br>public void setFont();</br>
<br>}</br>

<br>// Jadwal //</br>
<br>import java.util.Date;</br>
<br>public class Jadwal{</br>
	<br>private Date jam;</br>
	<br>private Date tanggal;</br>
	<br>private Date hari;</br>
	<br>public Jadwal(Date jam, Date tanggal, Date hari){</br>
		<br>this.jam = jam;</br>
		<br>this.tanggal = tanggal;</br>
		<br>this.hari = hari;</br>
	<br>}</br>
	<br>public Date getJam(){</br>
		<br>return jam;</br>
	<br>}</br>
	<br>public Date getHari(){</br>
		<br>return hari;</br>
	<br>}</br>
	<br>public Date getTanggal(){</br>
		<br>return tanggal;</br>
	<br>}</br>
	<br>public String toString(){</br>
		<br>return "Blablabla";</br>
	<br>}</br>
<br>}</br>
<br>// Task //</br>
<br>public class Task implements Customizable{</br>
	<br>private Jadwal jadwal;</br>
	<br>private String jenis, status, deskripsi, judul;</br>
	<br>public void setStatus(){</br>
		<br>this.status = "Belum";</br>
	<br>}</br>
	
<br>}</br>



import javafx.concurrent.Task;

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author SONY
 */
public class Reminder extends task {
    Jadwal jadwal;
    Task task;

    public Reminder(Jadwal jadwal, Task task) {
        this.jadwal = jadwal;
        this.task = task;
    }

    public Jadwal getJadwal() {
        return jadwal;
    }

    public void setJadwal(Jadwal jadwal) {
        this.jadwal = jadwal;
    }

    public Task getTask() {
        return task;
    }

    public void setTask(Task task) {
        this.task = task;
    }

    @Override
    public String toString() {
        return "Reminder{" + "\njadwal=" + jadwal + "\ntask=" + task + '}';
    }
    
    public void setUbahStatus(){
        super (getEdit());
    }
    
    public void setRepeat(){
        
    }
    
}
